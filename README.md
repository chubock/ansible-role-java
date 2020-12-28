Java
=========

A Role to install Java.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

    jdk_url: where to downloads JDK package from. default: https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_linux-x64_bin.tar.gz
    target_path: where to install Java. default: /opt/java/jdk-11
    java_home: where to put default link and set $JAVA_HOME environment variable. default: /opt/java/default

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: chubock.java, target_path: /var/lib/java/jdk-11, java_home: /var/lib/java/default }

License
-------

BSD
