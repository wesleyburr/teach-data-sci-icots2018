Notes from workshop with Mine & Colin

Getting Started & Computing
----------------------------
* rstudio.cloud - free for academic (teaching) use moving forward
* memory issues (tomorrow)

* using a Rmd interactive document on the first day - one small change = "coding"
* versus a notebook? (didn't ask)
* introducing the concept on the first day is better than using a Shiny interface and hiding the guts
    - motivation for what will be possible
    - need to build the course backwards, from the "outcomes" at the end, to what we start with on Day 1

Reproducibility
----------------
* scriptability - some good notes on how to make it clear
* literate programming (Donald Knuth)

Github
---------------
* being on the wrong repo when issuing a **pull** request gives the base issue
* no easy workaround
* when using Git in RStudio.cloud, need to initialize global Git options 
    * how far does this spread? project? all of your account? **currently project-specific** (feature request atm)
    * have to login to GitHub every time you push
    * caching of authentication information possible - Colin showed syntax
    
RStudio Cloud Intro
--------------------
* project installs are per-project
* can create a base project with an environment that can stay static through the term (Mine's: **All about that base**)
* avoids the install necessity

* teach R by osmosis, constant reinforcement
* Concurrency is an issue - can't have multiple people connected at once to a given project - issue for marking unless GitHub is used
* limits to numbers of workspaces + repositories, can request more for Academic use

GitHub for Education
-----------------------
* GitHub Classroom
* one repo per student/team per assignment
* repos are fungible - get lots, use lots
https://education.github.com/discount_requests/new

* to be able to use the API requires tokens
    - Developer Settings
    - Personal Access Token
    - create, then use it via ghclass (R Package)
    
ghclass
--------------
* check_user_exists() - vectorized, GitHub usernames
* get_members(), get_pending_members()
* default state in an org is 'Member' - **way** too much permission by default - **lock it down**
* get_repos() - can pull a list, filter it, then allow pushing material to all specific repos (e.g., hw01-)
* need to pull repos using HTTPS, not SSH
* **force students to always be working in the course workspace**
* **ISSUE** - if the auth fails, the git clone fails, but the project still creates 
* the cogwheel doesn't obviously tie to closing itself (UI)

* team stuff is quite easy - create_teams(), create_team_repo(), etc.
