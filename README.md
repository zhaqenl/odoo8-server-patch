odoo8-server-patch
==================

This is a `process_python` function patch for the
`/opt/odoo8/odoo8-server/openerp/service/server.py` file, for those that use
`emacs` as their text editor and those that develop using odoo 8’s
`--auto-reload` option, at the same time. Not applying this patch results in an
uncaught `IOError` due to emacs generating `*.py` files that start with `.#`,
hence the file not being found.
