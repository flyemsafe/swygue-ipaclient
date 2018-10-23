Role Name
=========

Enrolls or remove a host in a IDM realm.

Requirements
------------

Working IDM server.

Role Variables
--------------
* List of IDM servers is used to populate /etc/resolve
 ```
ipaclient_dns_servers:
 - server1
 - server2
```

* Set to False to register or True to Unregister from IDM server.
```
ipaclient_remove: False
```
* Force ipa-client-install --hostname <name>
```
ipclient_ipa_force_hostname: False
```

* Force the host to join even if it is already enrolled with --force-join.
```
ipaclient_ipa_force_join: True
```
* Force use of --request-cert to request cert for the macine.
```
ipaclient_ipa_request_cert: False
```

* Configure firefox to use IPA domain credntials with --configure-firefox.
```
ipaclient_ipa_configure_firefox: False
```
* Other Variables
```
ipaclient_dns_search_domain:
ipaclient_join_account:
ipaclient_join_password:
ipaclient_ipa_server:
ipaclient_ipa_domain:
ipaclient_ipa_realm:
```

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
