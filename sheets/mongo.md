Index
-----

* [Shell](#shell)
* [Query](#query)

Shell
-----

Reference: [here](https://docs.mongodb.org/manual/reference/mongo-shell/)
Here's a list of probably the most useful commands:
* `show dbs` to list dbs
* `use <db>` to use a db (can also do `mongo <db>`)
* `show collections` to list all collections of current db

Query
-----

* Nested field: `field1.field2.field3`
* Field existence: `<field>: {$exists: <boolean>}`
* Counting: `.count()`
