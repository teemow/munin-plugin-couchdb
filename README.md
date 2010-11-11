# Munin plugins for CouchDB

Some simple plugins that collect data from couchdb stats.

## Dependencies

 * Node.js >= 0.2.0
 * Cradle >= 0.2.2
 * CouchDB >= 1.0.1

## Installation

Clone this repository and link the plugins to /etc/munin/plugins/.

    sudo ln -s /etc/munin/plugins/couchdb_database_io couchdb_database_io

This assumes that node is in your PATH and that the cradle package is installed.
