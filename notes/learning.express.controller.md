---
id: 6pwyibv8wg82qexq38t0tbw
title: Controller
desc: ''
updated: 1671458918430
created: 1671458918430
---

- controller method
```js

exports.getTest("/", (req,res) => {
    res.status(200).json({success: true, msg: "get all data"})
})

exports.postTest("/", (req,res) => {
    res.status(200).json({success: true, data: "create a test data"})
})
```

- route file
```js
const express = require("express");
const router = express.Router();
const { getTest, postTest } = require('./path-to-controller')

router.route("/").get(getTest).post(postTest)
router.route("/:id").get(blabla).put(blabla).delete(blabla)

module.exports = router
```
