Node Deployment
====================

Disclaimer: These files and their descriptions are very specific to my project setup. They will not work on your setup. They are primarily here for me to keep centralised, so I can grab them for each new project and to share the techniques I have used.

Jakefile.js
--------------------

This file lives in the project root. It is called by the post-receive hook and does most of the work.


post-receive
--------------------

This is the git post-receive hook. Place it in the hooks directory in the git reposity of the project.


npm-depends.json
--------------------

This is a sample json document outlinining the npm packages requried by the app. This file lives in the site root /config


props.json
--------------------

This is a sample json document outlining the build properties. It also lives in the site root /config


site.Sitename-state
--------------------

This is the upstart daemon config. Place it in /etc/event.d/. State should be live/dev.


monitrc
--------------------

This is the monit config. Place it in /usr/local/etc/monitrc. The all of the sites to be monitored can be placed in this monolithic file.