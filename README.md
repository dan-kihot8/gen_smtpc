gen_smtpc
=============

`gen_smtpc` - is very simple smtp client for erlang.

Usage
--------------

Add `gen_smtpc` to your `rebar.config`:

```erlang
%% Dependencies
{deps, [
   {gen_smtpc, ".*", {git, "git://github.com/dan-kihot8/gen_smtpc.git"}}
   ]
}.
```

And send mail from your `erlang` application:

```erlang
application:start(gen_smtpc),
Options = [{use_ssl, true}, {host, "smtp.gmail.com"}, {port, 465}]),
gen_smtpc:send({"usermail@gmail.com", "password"}, "user2@gmail.com", "Subject", "Mail body", Options).
```

Contribute
--------------

  * Fork [gen_smtpc](https://github.com/OtpChatBot/gen_smtpc)
  * Make changes


License
--------------

Apache License Version 2.0.
