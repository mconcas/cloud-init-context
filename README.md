CloudInitContext
================

Contextualize WNs on INFN-Torino Tier2 with CloudInit
This is a repository for every file and script needed to create
the user-data MIME archive for workernodes.

Warning
-------

In the folder 'sensitive-data' are stored ssh-keys and 
other configuration files containing passwords, likely not to be propagated publicly.
Informations should be embedded in the archive at build time.

Every other needed file can be found in 'CloudInitFiles'.
This folder could go into a web server.
 
User data can be:
  - embedded from local folder (should be the case for sensitive data)
  - embedded from web server
  - fetched from web server at boot (convenient to avoid large user-data files)  

