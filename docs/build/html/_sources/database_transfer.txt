.. _database_transfer:

Database Transfer
==================
The database transfer tool enables an administrator to migrate their Moodle site from one database to another, for example from MySQL to Postgres.

The tool is currently classed as an experimental feature and may be found in *Settings > Site administration > Development > Experimental > Database migration*. There is also a command line script in admin/tool/dbtransfer/cli/migrate.php.

The dbtransfer tool uses the XMLDB schema definitions from Moodle and installed plugins to retrieve the data from one database and transfer it another.

Some troubles you may find when using this tool:

    * If there is any object in the current database (columns, tables,...) not included in the XMLDB schema the dbtransfer won't be executed until these objects are removed (this may happen if Moodle has been upgraded from earlier versions).
    * If there is some wrong encoded data in the current database the transfer will crash; in that case find and fix the troublemaking data and launch de dbtranfer tool again.
    * If you are trying to migrate a big instance it will take a while, and there can be set some timeout (database, PHP, Apache) that can break the migration. 




