---
title: "About"
date: 2024-10-18T15:44:00-04:00
---

## Introduction
The internet has turned to shit. All I wanted to know was when the next season
of a series I was interested in watching would be available on my streaming
services. What I got were articles which gave me the runaround while serving
me so many ads that my phone would heat up and my browser would slow to a
crawl. It wasn't always this way. There was a time when people would put
up a web page to share an interest or to inform people. That's what I am
trying to do. A no frills quick to load page which just lets you know when
a series is going to start.

## How to Contribute
You can contribute to this website by submitting updates to [the github
repository](https://github.com/devries/shows). To make contributions, fork the
repository, make your changes, and submit a pull request.

To add a new series simply
create a file in the [data/series](https://github.com/devries/shows/blob/main/data/series)
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
of the next year. Please use the existing files for reference.

To update a series, you can edit the existing file. 
