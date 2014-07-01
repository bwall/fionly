fionly
======

Prints out the first instance of a line from input


Usage
=====
    $ fionly -h
    usage: /usr/local/bin/fionly [-h] [-v] [path]

    Prints out the first unique instance of a line

    positional arguments:
      path           Paths to files to scan (if not supplied, stdin is the file
                     being read)

    optional arguments:
      -h, --help     show this help message and exit
      -v, --version  show program's version number and exit

    /usr/local/bin/fionly v1.1.0 by Brian Wallace (@botnet_hunter)

If you wanted to see all the IPs from your Apache log as they come in:

    tail -F /var/log/apache2/access.log | cut -d ' ' -f 1 | fionly
