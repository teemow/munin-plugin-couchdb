# Munin plugins for CouchDB

Some simple plugins that collect data from couchdb stats.

## Dependencies

 * Node.js >= 0.2.0
 * Cradle >= 0.2.2
 * CouchDB >= 1.0.1

## Installation

Clone this repository and link the plugins to /etc/munin/plugins/.

    git clone git://github.com/teemow/munin-plugin-couchdb.git
    cd munin-plugin-couchdb
    sudo ln -s /path/to/my/repository/couchdb_database_io /etc/munin/plugins/couchdb_database_io

This assumes that node is in your PATH and that the cradle package is installed in a vendor directory.

    npm bundle vendor

If node is eg installed in /usr/local/ – add this to /etc/munin/plugin-conf.d/munin-node.

    [couchdb_*]
    user root
    env.PATH /usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin

