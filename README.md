# Using git submodules
To pull all of the repo including the submodules use the command `git clone --recursive  http://github.com/<your repo>`
To download all of the updates to an existing repo use the command `git submodule update --remote --recursive --merge`

When changing code in the submodule, cd into that directory and run your git commands.
Once that code is committed, cd back into the top level directory and run `git submodule update`.

# Run with Docker
From the top level directory, run the command `docker compose up`. 

You can also build the images individually with `docker build -t <tag:version> .` (be sure to `cd` into the repo with the dockerfile in it.
You can then run the individual images with `docker run -p <hostport:app-port> <imagename>`

# Ports
Events - 9000
Customers - 9001
Registrations - 9002
Auth - 8081
Gateway - 8080 (/api/)
React App - 3000
