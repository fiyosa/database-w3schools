# W3Schools Database

- [Documentation](https://www.w3schools.com/sql/default.asp)
- [Simulation](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all)

```sh
mysqldump -u root -p --routines --skip-comments w3schools > "C:\Users\fys\Downloads\dumpMYSQL.sql"
```

```sh
mysql -u [username] -p [database_name] < [file_path]
```

## if error constraint "users_pkey"
SELECT setval(pg_get_serial_sequence('users', 'id'), coalesce(max(id)+1, 1), false) FROM users;