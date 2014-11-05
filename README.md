nodeBrowserLog
==============

send console.log from node to browser-console via local server

## Installation

  npm install nodefirebug --save

## Usage
  var nbl = require('nodebrowserlog');

  ### configure and start the server:
  > option:1
  nbl.config({
    "port":6000,
    "type": "json"
  });
  nbl.startServer();

  >option:2
  nbl.startServer(7777); //type: "html"

  >option:2
  nbl.startServer(); //port: 9090, type: "html"

  ### log
  nbl.log(obj);
  nbl.log(arr);