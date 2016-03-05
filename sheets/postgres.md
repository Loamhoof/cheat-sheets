Index
-----

* [Shell](#shell)
* [Export](#export)
* [Import](#import)

Shell
-----

To get the full list of commands, use `\?`.
Here's a list of probably the most useful commands:
* `\d` to list tables, sequences and views
* `\dt` to get the list of tables only
* `\d+ <table>` to describe a table (with keys, constraints, indexes and everything)
* `\timing` to time all your queries
* `\x on/auto/off` to toggle the expanded output mode (when lines are too long, the results are displayed one by one with each field on a new line)
* `\! <command>` to execute a UNIX shell command inside your psql shell
* `\!` to start a new UNIX shell inside your psql shell (exiting the UNIX shell will bring you back in the psql shell)

If you want to enable `\timing` and `\x auto` by default, put them in a `~/.psqlrc` file.

Export
------

Exporting as a csv:
`\copy some_table TO '/path/to/csv' DELIMITER ';' CSV HEADER`


Import
------

Importing a csv:
`\copy some_table FROM '/path/to/csv' DELIMITER ';' CSV HEADER`
