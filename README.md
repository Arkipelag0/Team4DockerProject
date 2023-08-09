# Using git submodules
When changing code in the submodule, cd into that directory and run you git commands.
Once that code is committed, cd back into the top level directory and run `git submodule update`.

# Run with Docker
From the top level directory, run the command `docker compose up`.

# Ports
Events - 9000
Customers - 9001
Registrations - 9002
Gateway - 8080 (/api/)
