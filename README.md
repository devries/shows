I just wanted to know when a series was going to be streaming. Why is that
so hard to look up? Why do web pages feed me advertisements rather than
answers? So I decided to make this web page.

This is (hopefully) live at https://shows.unnecessary.tech/. 

Feel free to fork this repo and add or update series information. The series
data files should be stored in the [data/series](data/series) directory.  
To add a new series simply
create a file in the [data/series](data/series)
directory with the name in the format `title_sN.yaml` where `title` is the
series title in all lowercase with "_" characters instead of spaces, and
`N` is the season number. The file should have the following format:

```
---
  name: "Daredevil: Born Again"
  service: Disney+
  season: 1
  date: 2025-03-31
  displayDate: March 2025
  universe: Marvel
```

The `name`, `service`, `season`, and `date` fields are mandatory and the 
`displayDate` and `universe` are optional. If you only have an approximate
date you should fill in the `displayDate` field and then set the `date` to a
value at the end of that approximate period. For shows that only have a year
in which they are supposed to start, we set the `date` field to the January 1
of the next year. The format for the `date` field is `YYYY-MM-DD` however. The
`service` field indicates which streaming service the show will be on. We
currently have pages for the following services:

- Amazon Prime
- Apple TV+
- Disney+
- HBO Max
- Hulu
- Netflix
- Paramount+
- AMC+

Feel free to add a service if it is missing. The `universe` tag is provided to
links series from the same universe. We currently have the following universes:

- Marvel
- Star Trek
- Star Wars

Please use the existing files for reference. To update a series, you can edit
the existing file.

The web page is build using [Hugo](https://gohugo.io/) which
you can install on your own computer if you want to preview your edits. Just run
`hugo server` from the command line in the root directory of the project and
you should see a preview at http://localhost:1313.
