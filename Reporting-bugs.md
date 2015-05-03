# Reporting bugs
--------------------------------------------

If you have found a bug in *guh*, please create a new issue with the "**bug**" label in the related repository:

* *guh*-daemon - [https://github.com/guh/guh/issues](https://github.com/guh/guh/issues)
* *guh*-cli - [https://github.com/guh/guh-cli/issues](https://github.com/guh/guh-cli/issues)
* *guh*-webserver - [https://github.com/guh/guh-webserver/issues](https://github.com/guh/guh-webserver/issues)
* *guh*-webinterface - [https://github.com/guh/guh-webinterface/issues](https://github.com/guh/guh-webinterface/issues)

If you don't know where the bug occurs, please use the *guh*-daemon issues link.

## Steps to find out whats wrong

1. In order to find out what's wrong it's very helpful to start the *guh* daemon in the foreground:

        $ guhd -n

    Now you can follow the debug output of the core and check what's going on.

2. Make shore, there is only one instance of `guhd` running on your system, otherwise they will block each others ports.
3. Try to use the [guh-cli](https://github.com/guh/guh/wiki/guh-cli) (which is communicating directly with the JSON-RPC API)
4. If you have made an upgrade of guh, a plugin configuration might have changed. Try to reset the configurations (see [here](https://github.com/guh/guh/wiki/Configuration)) and restart the guh daemon.


## Questions, Comments, and Troubleshooting

If you have any questions, you can get help in following locations:

* [guh-mailinglist](https://guh.guru/cgi-bin/mailman/listinfo)
* [#guh]() IRC channel on [freenode.net](https://freenode.net/)

If you need any help with *guh* or if you are not shore if something is really a bug, or how to reprodue it please use one of the above channels.








