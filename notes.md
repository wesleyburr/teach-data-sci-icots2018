Notes from workshop with Mine & Colin

Getting Started & Computing
----------------------------
* rstudio.cloud - free for academic (teaching) use moving forward
* memory issues (tomorrow)

* using a Rmd interactive document on the first day - one small change = "coding"
* versus a notebook?
* introducing the concept on the first day is better than using a Shiny interface and hiding the guts
    - motivation for what will be possible
    - need to build the course backwards, from the "outcomes" at the end, to what we start with on Day 1

Reproducibility
----------------
* scriptability - some good notes on how to make it clear
* literature programming (Donald Knuth)

Github
---------------
* being on the wrong repo when issuing a **pull** request gives the base issue
* no easy workaround
* when using Git in RStudio.cloud, need to initialize global Git options 
    * how far does this spread? project? all of your account? **currently project-specific** (feature request atm)
    * have to login to GitHub every time you push
    * caching of authentication information possible
    
RStudio Cloud Intro
--------------------
* project installs are per-project
* can create a base project with an environment that can stay static through the term
* avoids the install necessity

* teach R by osmosis, constant reinforcement
* Concurrency is an issue - can't have multiple people connected at once
* limits to numbers of workspaces + repositories
