**DOCUMENTATION**
==============

Vars
----

None

HowTo
-----

We can use this role using its two tags.

Stop the cluster nodes:

```bash
$ ansible-playbook playbook.yaml -i inventory --tags "stop"
$ #This will stop all the nodes in sequence, stopping, before shutdown the node, some services.
```

Start the cluster nodes:

```bash
$ ansible-playbook playbook.yaml -i inventory --tags "start"
$ #This will start all the services in the nodes and let them ready to use again.
```
