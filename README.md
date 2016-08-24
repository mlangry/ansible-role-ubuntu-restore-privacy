mlangry.ubuntu-restore-privacy
=========

If you're an Ubuntu user and you're using the default settings, each time you start typing in Dash (to open an application or search for a file on your computer), your search terms get sent to a variety of third parties, some of which advertise to you.

Ubuntu should protect user privacy by default. Since it doesn't, this ansible role disable the parts of Ubuntu which are invasive to your privacy.

Note: This privacy problem only affects Unity. If you use GNOME (sudo apt-get install gnome-shell) or any other desktop environment, or if you run an Ubuntu derivative like Linux Mint, Xubuntu, Kubuntu, etc., you won't have this problem.

Requirements
------------

None.

Role Variables
--------------

````yaml
ubuntu_privacy_min_version: 12.10
ubuntu_privacy_gsettings_path: /usr/bin/gsettings
ubuntu_privacy_canonical_schema: com.canonical.Unity.Lenses
````

Dependencies
------------

None.

Example Playbook
----------------

````yaml
- hosts: desktopUbuntu
  roles:
     - mlangry.ubuntu-restore-privacy
````

License
-------

MIT
