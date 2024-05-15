# node-red-contrib-keysight

This is a fork of the node-red-contrib-bb3 package, modified to be compatible with Keysight products as well.
The difference is between bb3 and Keysight at the query messages. The Keysight sendign the messages with \n instead of \r\n

## Install

To install - either use the manage palette option in the editor, or change to your Node-RED user directory.

        cd ~/.node-red
        npm install node-red-contrib-keysight

## Features

Supported keysight related nodes:

- `keysight-connect`: Connects to keysight using TCP.
- `keysight-disconnect`: Disconnects from keysight.
- `keysight-command`: Executes SCPI command.
- `keysight-query`: Execute SCPI query.

Also, there are two nodes for simple event based communication inside Node-RED flows. You can emit events with `bb3-emit-event` and catch it with `bb3-on-event` from any node in your project.

----- ORIGINAL REPOSITORY README -----

# node-red-contrib-bb3

A [Node-RED](http://nodered.org) nodes to work with [EEZ BB3](https://www.envox.hr/eez/eez-bench-box-3/introduction.html).

## Install

To install - either use the manage palette option in the editor, or change to your Node-RED user directory.

        cd ~/.node-red
        npm install @eez-open/node-red-contrib-bb3

## Features

Supported EEZ BB3 related nodes:

- `bb3-connect`: Connects to EEZ BB3 using TCP.
- `bb3-disconnect`: Disconnects from EEZ BB3.
- `bb3-command`: Executes SCPI command.
- `bb3-query`: Execute SCPI query.

Learn about supported SCPI commands and queries from here https://www.envox.hr/eez/eez-bench-box-3/bb3-scpi-reference-manual/bb3-scpi-introduction.html.

Also, there are two nodes for simple event based communication inside Node-RED flows. You can emit events with `bb3-emit-event` and catch it with `bb3-on-event` from any node in your project.
