# Time for a Little Magic Trick

trying to open Joker.db in database software reveals it's not actually a database

`binwalk Joker.db`
reveals jpg data in database file

`binwalk -D='.*' Joker.db`
extracts jpg image of a joker card with flag written at the top.
