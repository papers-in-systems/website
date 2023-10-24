# website

this repo contains the [papersin.systems](https://papersin.systems) website

## How to: add a session

Create a new markdown document in the `_sessions` directory. Make sure to include the following "frontmatter" metadata:

```
---
layout: session
title: # the pithy title
paper_title: # the full rambling title, including subtitle, etc
paper_author: # academic citation style "et al" or the plain language author's name
paper_year: # full year the work was published
paper_link: # link to a pdf, conference site, non-commercial book link, etc
presenter:
  - name: # presenter's preferred name
    link: # social media link or home page
registration: # link to the tito page for this session (get from Ruth)
date: # full date (YYYY-MM-DD) of the session
miro: # name of high resolution PDF export from Miro board. This should be the same name as the corresponding session markdown document.
slug: # Summary for upcoming page.
---

description / excerpt / abstract of the paper
```

## How to: add a page to the header

Create a new markdown document in the `_/pages` directory, and add it to the `header_pages` section in `_config.yml`.

## How to: develop locally

Clone the repo and run `docker compose up` or `podman compose up`. This will build a docker image and start the jekyll devserver, which will live-reload on most changes. Note, changes to `_compose.yml` require a manual restart with `ctrl-c` and re-running the `docker compose up` command.

## Todo

- [ ] Review content for previous sessions.
- [ ] Add content for proposing a session.
- Add Miro board high resolution PDF export files for:
  - [ ] Feb 2023
  - [ ] Mar 2023
  - [ ] Jul 2023
  - [ ] Aug 2023 
  - [ ] Sep 2023
  - [ ] Oct 2023  
