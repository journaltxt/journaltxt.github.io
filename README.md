[Journal.TXT @ GitHub](https://github.com/journaltxt)

# Journal.TXT - Single-Text File Journals - The Human Multi-Document Format for Writers

Write your journal in a single-text file. Example:

``` text
--- 
year:  2017
month: July
day:   Wed 19
---
Let's reinvent push-button publishing on the internets! 
Use a single-file for your journal / diary / blog. That's it.
---
day:   Thu 20
---
Crazy idea? Let's put up a website and a example blog auto-generated from journal.txt.
---
day:   Fri 21
---
Did you know? The single-file format works great for advent calendars 
or beer-of-the-day calendars.
---
day:    Sat 22
---
Let's add another example. A diary about the Oktoberfest 2016. Prost. Cheers.
---
day:    Sun 23
---
Let's rest.
```

How does it work?

The single-text file is a series of meta data and text blocks. 

### Dates

Use the meta data block for adding the date. In the first meta data block 
you need a "full" date, that is, year/month/day e.g.:

```
year: 2017
month: July
day:   Wed 19
```

or

```
date: 2017-07-19
```

In the following entries you only need to add what changes e.g. still in the same month as yesterday? 
just add a day entry (and the computer will calculate the full date) e.g.:

```
day: Thu 20
```

or

```
day: 20
```

Use any of these date entries:

- **year** or **y**   --  year
- **month** or **m**   -- month  (use  1,2,3,etc. or Jan,Feb,Mar or January,February)
- **week**  or **w**    -- week  (use 1,2,3, etc.)
- **day**   or **d**    -- day (use 1,2,3...31  or Wed 19, Thu 20,...)
- **julian** or **j**    -- julian day (use 1,2,3..364,365)

Bonus:  Add the year or month to the file name. If you use a filename in the YYYY-MM-title.txt or YYYY-title.txt 
or format than journal.txt will auto-add the year (and month) from the filename.


### Titles

Note: You do NOT need a title for you entries and you do NOT need a title for your journal (use journal.txt if you like). 

If you use a differnt name e.g. austria.txt or 2017-oktoberfest.txt than journal.txt will auto-add the title 
from the filename.

By default the journal entries get auto-titled. Example:

- Day #1 - Wed July 19
- Day #2 - Thu July 20
- Day #3 - Fri July 21

If you add a title - the title by default gets added e.g.

- Austria - Day #1 - Wed July 19
- Austria - Day #2 - Thu July 20
- Austria - Day #3 - Fri July 21

Note: You can always customize the title format.  FUTURE (To be done). 



## Bonus:  Single-Source for Blog Posts & Status Tweets / Toots

You can add tweets (or toots) to your journal.TXT. Use a "generic" block in the [Text with Instructions (.texti)](https://texti.github.io/) format. 
Example:

``` text
:::::: Tweet :::::::  
:: New! Journal.TXT - Single-Text File Publishing - 
:: The Human Multi-Document Format for Writers - Blogging Reinvented https://journaltxt.github.io  
```

or use the "long" block form:

``` text
:::::: Tweet ::::::::::::
New! Journal.TXT - Single-Text File Publishing - 
The Human Multi-Document Format for Writers - Blogging Reinvented https://journaltxt.github.io
::::::::::::::::::::::
```

If configured your Journal.TXT processor will publish (auto-build) your blog AND publish your (new) tweets (on twitter)
all from a single-text source file, for example.




{% include_relative samples/README.md %}



## License

The Journal.TXT format and conventions are dedicated to the public domain.
Use it as you please with no restrictions whatsoever.

## Questions? Comments?

Send them along to the [wwwmake mailing list/forum](http://groups.google.com/group/wwwmake). Thanks.
