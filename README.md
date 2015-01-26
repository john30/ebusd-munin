# ebusd-munin
Collection of munin plugins related to ebusd.
These plugins can easily be used to feeda munin node with data from a local ebusd instance.
Personally, I use them for checking mainly temperatures, pressures and earned energy of my heatpump. Looking at the graphs produced by munin I find it rather easy to know what's going on in the heatpump.

# Installation:
- prerequisite is of course a running munin installation on the local host
- to install the plugins:
  - git checkout https://github.com/john30/ebusd-munin.git
  - chmod a+x ebusd-munin/plugins/*
  - sudo cp ebusd-munin/plugins/* /etc/munin/plugins
  - sudo munin-node-configure --shell
  - run all "ln -s" commands printed by munin-node-configure
  - sudo service munin-node reload
  - that's it
