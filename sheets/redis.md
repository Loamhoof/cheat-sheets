Index
-----

* [Backup](#backup)

Backup
------

Redis data is located in `/var/lib/redis/dump.rdb`. Save that file.

To restore it, stop the server, replace that file and restart it.

Bonus: to compress/uncompress the backup, `bzip2 dump.rdb` & `bunzip2 dump.rdb.bz2`.
