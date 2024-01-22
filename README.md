# Setup
1. install docker desktop locally on your machine
1. clone this repo
1. (linux/mac/wsl) from the cloned repo directory run the command `bin/setup`
1. (windows) create a folder in root of project called repos
1. (windows) run each of the following git commands
1. (windows) `git clone git@github.com:bfurner27/earthquakes_poc_data.git data_entry`
1. (windows) `git clone git@github.com:bfurner27/earthquake_poc_frontend.git frontend`
1. (windows) `git clone git@github.com:bfurner27/earthquake_poc_backend.git backend`

# Running project
1. run `docker compose build`
1. run `docker compose up -d`

# See Frontend
1. in browser navigate to http://localhost:2402/

# See Backend Docs
1. in browser navigate to http://localhost:2401/docs

# Initially Seed The DB
1. follow instructions [here](https://github.com/bfurner27/earthquakes_poc_data/blob/main/README.md)
* only run the seed scripts once since deduping is not yet supported in the db (it will upload duplicates if you run it more than once)
