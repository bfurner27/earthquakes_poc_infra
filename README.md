# Setup
1. install docker desktop locally on your machine
1. clone this repo
1. (linux/mac/wsl) from the cloned repo directory run the command `bin/setup`
1. (windows) create a folder in root of project called repos
1. (windows) run each of the following git commands
1. (windows) `git clone git@github.com:bfurner27/earthquakes_poc_data.git -o data_entry`
1. (windows) `git clone git@github.com:bfurner27/earthquake_poc_frontend.git -o frontend`
1. (windows) `git clone git@github.com:bfurner27/earthquake_poc_backend.git -o backend`

# Running project
1. run `docker compose build`
1. run `docker compose up -d`

1. seed the db by extracting the zipped data into the directory repos/data
1. run the data_entry linux container `docker compose run data bash`
1. run the command `python3 update.py --file-path data/Countries.geojson --data-type country`
1. run the command `python3 update.py --file-path data/Earthquakes.geojson --data-type earthquake`
\* currently deduping is not supported so ensure you only run the above commands once to initially seed the db