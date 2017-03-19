sphero_ros
==========

checkout the [docs](http://mmwise.github.com/sphero_ros)

=======
## Installation
Installation is now based on catkin:

      cd <ws>/src
      git clone https://github.com/mmwise/sphero_ros
      cd <ws>
      catkin_make
      catkin_make install
      source <ws>/install/setup.bash
      ...


# Marc's notes

* install bluepy: `sudo pip install bluepy`
* enable discovery for non-root: `sudo setcap 'cap_net_raw,cap_net_admin+eip' /usr/local/lib/python2.7/dist-packages/bluepy/bluepy-helper`
* what the current version expects in `/cmd_vel` appears to be `cm/s` and not `m/s` as it should. Also, setting the heading doesn't seem to work.
* sensor information only arrives when and if BB8 is moving. Otherwise, no odometry etc is working.
