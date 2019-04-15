# monitoring-slave

Setup for deploying telegraf nodes to servers.

To use run:

```shell
$ git clone https://github.com/frederiksberg/monitoring-slave
```

Define your master-node intrinsics in a .env file:
```shell
$ cp example.env .env
$ vim .env
```

Deploy node by running
```shell
$ make deploy
```
Or if you want to see debug output for testing:
```shell
$ make run
```

You can tear down the node again by running
```shell
$ make kill
```

And clean up stopped nodes by running
```shell
$ make clean
```

## Dependencies
* **make**
* **docker**
* **docker-compose**
