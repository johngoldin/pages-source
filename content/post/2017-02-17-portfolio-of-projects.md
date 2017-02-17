---
title: Portfolio of Projects
date: '2017-02-17'
categories:
  - R
  - personal
tags:
  - R
---
<!--- created with this command:
# blogdown::new_post("Portfolio of Projects", categories = c("R", "personal"), tags = c("R"), rmd = FALSE)  --->
One motivation for creating this blog was to display a portfolio of projects that I have worked
on in the last year or so. I'll list projects here.
Eventually I hope to create pages that elaborate each project.

### The Diary of Samuel Pepys

Each morning I read an entry from
[The Diary of Samuel Pepys](http://www.pepysdiary.com/) at a wonderful
site created by [Phil Gyford](http://www.gyford.com/). Pepys kept the diary for about ten years during the 1660's.
Inspired by a post by 
[Julia Silge](http://juliasilge.com/blog/Life-Changing-Magic/), 
I did some simple
text processing on the diary. That became the
occasion for my first shot at creating a Shiny app.
The result is available [here](https://goldin.shinyapps.io/Search_Pepys/).

I had an opportunity to chat with Julia at the RStudio Conference in Orlando. She gave me some suggestions
for some additional things I might do with the diary.

### Souvenirs of My Walks
I have always loved to walk. When I retired in 2011 I went on a walking binge.
At the same time, I discovered that a GPS trace
could be a fun souvenir of my walks.
An [article](http://mhermans.net/hiking-gpx-r-leaflet.html) I found via [R Bloggers](https://www.r-bloggers.com/) led me
to try to keep track of my walks more systematically.
After doing some research on how to access the Flickr API from R,
I was able to display my photos from Flickr on the GPS trace in a Leaflet map.
The result is a Shiny app [here](https://goldin.shinyapps.io/Walks/).
I don't thnk this is of great interest to a stranger, but for me it is a fascinating
picture of my walks. I love to zoom in and see the detail of the map combined with the GPS trace and the photos.
Like a good souvenir, it triggers lots of memories. If I lingered on a bench additional squiggles appear
on the GPS trace showing where I stopped for a spell. I can also see my wrong turns.

