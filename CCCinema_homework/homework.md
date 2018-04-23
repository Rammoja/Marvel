# SQL Homework

The Dominion Cinema are having a Marvel Movie Marathon! They have asked you to help maintain their database of movies with times and attendees.

## To access the database:

First, create a database called 'marvel'

```
# terminal
createdb marvel
```

Next, run the provided SQL script to populate your database:

```
# terminal
psql -d marvel -f marvel.sql
```

Use the supplied data as the source of data to answer the questions.  Copy the SQL command you have used to get the answer, and paste it below the question, along with the result they gave.

## Questions

1. Return ALL the data in the 'movies' table.

SELECT * FROM movies;

id |                title                | year | show_time
----+-------------------------------------+------+-----------
 1 | Iron Man                            | 2008 | 19:55
 2 | The Incredible Hulk                 | 2008 | 18:40
 3 | Iron Man 2                          | 2010 | 21:55
 4 | Thor                                | 2011 | 16:35
 5 | Captain America: The First Avenger  | 2011 | 13:25
 6 | Avengers Assemble                   | 2012 | 22:05
 7 | Iron Man 3                          | 2013 | 23:10
 8 | Thor: The Dark World                | 2013 | 12:25
 9 | Batman Begins                       | 2005 | 14:00
10 | Captain America: The Winter Soldier | 2014 | 14:45
11 | Guardians of the Galaxy             | 2014 | 18:55
12 | Avengers: Age of Ultron             | 2015 | 20:40
13 | Ant-Man                             | 2015 | 13:50
14 | Captain America: Civil War          | 2016 | 21:30
15 | Doctor Strange                      | 2016 | 17:55
(15 rows)


2. Return ONLY the name column from the 'people' table

SELECT name FROM people;


 Yang Chen
 Ruairidh Grass
 Hannah Green
 Hamish Hoad
 Andrew Laughlin
 Jo Malo
 Duncan Marjoribanks
 Juan Mata Ruiz
 Paul McPhail Stevenson
 Sarah Murphy
 Katy Preston
 Richard Ramson
 Iain Rogerson
 Davinda Sanders
 Joe Stafford
 Daniel Stewart
 Luis Tejero
 Colin Tindle
 Rachel Westwater
 Andrew Smith
 Zsolt Podoba-Szalai
(23 rows)


3.Oops! Someone at CodeClan spelled Davina's name wrong! Change it to reflect the proper spelling (change 'Davinda Sanders' to 'Davina Sanders').





4. Return ONLY your name from the 'people' table.
5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
6. Create a new entry in the 'people' table with the name of one of the instructors.
7. Zsolt, has decided to hijack our movie evening, Remove him from the table of people.
8. Somehow the list of people includes two people named 'Andrew'. Change these entries to the proper names ('Jeff 4', 'Jeff 5')
9. The cinema has just heard that they will be holding an exclusive midnight showing of 'Guardians of the Galaxy 2'!! Create a new entry in the 'movies' table to reflect this.
10. The cinema would also like to make the Guardian movies a back to back feature. Update the 'Guardians of the Galaxy' show time from 18:55 to 21:30

## Extension

1. Research how to delete multiple entries from your table in a single command.
