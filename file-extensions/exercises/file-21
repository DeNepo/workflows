const util = require('util');
const path = require('path');
const fs = require('fs');
const tv4 = require('tv4');

const PROFILES_SCHEMA = require('../data/profile-schema.json');
const DATA_PATH = path.join(__dirname, '..', 'data', 'profiles-data.json');

const readFile = util.promisify(fs.readFile);
const writeFile = util.promisify(fs.writeFile);

const handlers = {
  create: async (req, res) => {
    const newProfile = req.body;

    try {
      const profilesDataString = await readFile(DATA_PATH, 'utf-8');
      const profilesData = JSON.parse(profilesDataString);

      newProfile.id = profilesData.nextId;
      profilesData.nextId++;

      const isValid = tv4.validate(newProfile, PROFILES_SCHEMA);

      if (!isValid) {
        const error = tv4.error;
        console.error(error);

        res.status(400).json({
          error: {
            message: error.message,
            dataPath: error.dataPath,
          },
        });
        return;
      }

      profilesData.profiles.push(newProfile);

      const newProfileDataString = JSON.stringify(profilesData, null, '  ');

      await writeFile(DATA_PATH, newProfileDataString);

      res.json(newProfile);
    } catch (err) {
      console.log(err);

      if (err && err.code === 'ENOENT') {
        res.status(404).end();
        return;
      }
    }
  },
  readAll: async (req, res) => {
    try {
      const profilesDataString = await readFile(DATA_PATH, 'utf-8');
      const profilesData = JSON.parse(profilesDataString);

      res.json(profilesData.profiles);
    } catch (err) {
      console.log(err);

      if (err && err.code === 'ENOENT') {
        res.status(404).end();
        return;
      }
    }
  },
  readOne: async (req, res) => {
    const idToUpdateStr = req.params.id;
    const idToUpdate = Number(idToUpdateStr);

    try {
      const profilesDataString = await readFile(DATA_PATH, 'utf-8');
      const profilesData = JSON.parse(profilesDataString);
      const selectedProfile = profilesData.profiles.find(
        (profile) => profile.id === idToUpdate,
      );

      res.json(selectedProfile);
    } catch (err) {
      console.log(err);

      if (err && err.code === 'ENOENT') {
        res.status(404).end();
        return;
      }
    }
  },
  update: async (req, res) => {
    const idToUpdateStr = req.params.id;
    const idToUpdate = Number(idToUpdateStr);

    const newProfile = req.body;
    newProfile.id = idToUpdate;
    const isValid = tv4.validate(newProfile, PROFILES_SCHEMA);

    if (!isValid) {
      const error = tv4.error;
      console.error(error);

      res.status(400).json({
        error: {
          message: error.message,
          dataPath: error.dataPath,
        },
      });
      return;
    }

    try {
      const profilesDataString = await readFile(DATA_PATH, 'utf-8');
      const profilesData = JSON.parse(profilesDataString);

      const entryToUpdate = profilesData.profiles.find(
        (profile) => profile.id === idToUpdate,
      );

      if (entryToUpdate) {
        const indexOfProfile = profilesData.profiles.indexOf(entryToUpdate);
        profilesData.profiles[indexOfProfile] = newProfile;

        const newProfileDataString = JSON.stringify(profilesData, null, '  ');

        await writeFile(DATA_PATH, newProfileDataString);

        res.json(newProfile);
      } else {
        res.json(`no entry with id ${idToUpdate}`);
      }
    } catch (err) {
      console.log(err);

      if (err && err.code === 'ENOENT') {
        res.status(404).end();
        return;
      }
    }
  },
  delete: async (req, res) => {
    const idToDeleteStr = req.params.id;
    const idToDelete = Number(idToDeleteStr);

    try {
      const profilesDataString = await readFile(DATA_PATH, 'utf-8');
      const profilesData = JSON.parse(profilesDataString);

      const entryToDelete = profilesData.profiles.find(
        (profile) => profile.id === idToDelete,
      );

      if (entryToDelete) {
        profilesData.profiles = profilesData.profiles.filter(
          (profile) => profile.id !== entryToDelete.id,
        );

        const newProfileDataString = JSON.stringify(profilesData, null, '  ');

        await writeFile(DATA_PATH, newProfileDataString);

        res.json(entryToDelete);
      } else {
        res.json(`no entry with id ${idToUpdate}`);
      }
    } catch (err) {
      console.log(err);

      if (err && err.code === 'ENOENT') {
        res.status(404).end();
        return;
      }
    }
  },
};

module.exports = handlers;
