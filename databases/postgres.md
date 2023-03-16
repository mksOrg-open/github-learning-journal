Installing with Homebrew

```sh
$ brew install postgresql
```

It will give you instructions on creating an initial database. When you do it will be "owned" by your username and create the `postgres` and `template1` databases.
Run the following to start the server.

```sh
$ brew services start postgresql # or "brew services run postgresql" to have it not restart at boot time
# or the pg_ctl command it mentions
```


To connect/use it, as your user:
```sh
$ psql postgres
```

You can see what other versions are available for install by running

```sh
$ brew search postgres
==> Formulae
check_postgres  postgresql ✔    postgresql@10   postgresql@11 ...
```