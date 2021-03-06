EMV: Credit Card Validation
===========================

An Erlang module for testing credit card numbers.

You can also run a credit card validation server. The configuration
can be found in config/server_config.erl

To start the server use:

```
$ mad com bun emv
$ ./emv
```

The validation example url is: <a href="http://localhost:8800/emv_server:validate?4019100110000006">http://localhost:8800/emv_server:validate?4019100110000006</a>

or in repl:

```
> emv:type("4019100110000006").
inn_visa
```

and Result:

```
{inn_visa,"4019100110000000",true}
```

Credits
-------

* Maxim Sokhatsky
