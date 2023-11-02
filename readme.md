## Open pgbouncer admin

1. Step 1: Set unix_socket_dir=/tmp in pgbouncer.ini.
2. Step 2: Connect using the Unix socket with user pgbouncer and no password:

```bash
$ psql --port=6432 --host=/tmp --username=pgbouncer --no-password pgbouncer
```

or 

You can access using postgres user and password

```bash
$ psql --port=6432 --host=/tmp --username=root pgbouncer
```

Enter password for `root`

or

```bash
$ psql --port=6432 --host=localhost --username root pgbouncer
```

Please make sure userlist.txt format is correct.

Example: 

```bash
"username" "password"
"root" "root"
```