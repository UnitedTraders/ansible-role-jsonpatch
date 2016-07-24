jsonpatch
=========

Adds `jsonpatch` command to edit JSON files on destination machine.

Updated file is written to destination pretty-printed with indent of 2 spaces and sorted keys.

Requirements
------------

Optional requirement is `commentjson` Python module. Makes command `jsonpatch` work with comments inside JSON.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - jsonpatch
      tasks:
         - jsonpatch: file=/path/to/file/on/server key="first.second" value="new value"
         - jsonpatch: file=/path/to/file/on/server key="first.list" value={{ list_var }}


License
-------

BSD
