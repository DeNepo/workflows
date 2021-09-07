const handlers = require('./handlers.js');
const express = require('express');

const router = express.Router();

router.get('/profiles', handlers.readAll);
router.get('/profiles/:id', handlers.readOne);
router.post('/profiles', handlers.create);
router.put('/profiles/:id', handlers.update);
router.delete('/profiles/:id', handlers.delete);

module.exports = router;
