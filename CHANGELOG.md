# 2013-June

  0.1.0: 2013-06-20
  
    Initial drop of code - to be used only in test/lab. The modules have hardcoded username/password 
    of "root/juniper1" for now.  The modules will be udpated in the near future to include arguments 
    (username/passwords) and will also support ssh-key environments.  This is *early*, so I appreciate
    any feedback, issues you find.  Feel free to open issues against this repo or contact me via
    email: jschulman@juniper.net, or on Twitter: @nwkautomaniac.
    
    This drop is also harded to use the path /usr/local/junos, so you will need to create that directory.
    This directory will contain subdirs: [log, packages, configs].  You should create those too.  There
    is a file in this repo called "catalog.yml".  This file is used by the sample junos/install_os.yml
    playbook.  You need to copy this file to /usr/local/junos/packages.
  

  0.1.1: 2013-06-20
  
    Removed the hardcoded root user/password and added support for args (user/password).  If user
    is not provided, then assumes $USER.  If password is not provided, then assumes ssh-key is active.

# 2013-July

  0.2.0: 2013-07-04
  
    Updated this repo to only include the Junos modules.  The sample tasks, playsbooks, etc., have
    been moved to the ansible-junos-demo repo.

  0.2.1: 2013-07-08
  
    Updated `junos_rescue` to include `action` argument.  You can now load, save, delete the
    Junos rescue configuration with this update
