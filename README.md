Java
=========

A Role to install Java.

Role Variables
--------------
There are 3 variables that defines where to download JDK package from, Where to install the package and where to create a link for installation location where JAVA_HOME environment variable refer to:

    jdk_url: where to downloads JDK package from. default: https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_linux-x64_bin.tar.gz
    target_path: where to install Java. default: /opt/java/jdk-11
    java_home: where to put default link and set $JAVA_HOME environment variable. default: /opt/java/default

Example Playbook
----------------

An example of a playbook overriding some of the variables:

    - hosts: servers
      roles:
         - { role: chubock.java, target_path: /var/lib/java/jdk-11, java_home: /var/lib/java/default }

License
-------

BSD
