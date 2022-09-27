# TAK Server Certificate Enrollment
## This script package will assist in setup of Certificate Enrollment on your TAK Server Docker Instance in just a few minutes.
### More info Here: https://atakhq.com/en/tak-server/cert-enrollment

1. Login as TAK Superuser and clone this repo to your machine

`su - tak`

`cd /tmp/ && git clone https://github.com/atakhq/tak-cert-enrollment-script.git && sudo chmod -R +x * /tmp/tak-cert-enrollment-script/`


2. Open a shell for your Docker container running TAK Server

`docker exec -it tak-server-tak-1 /bin/bash`


2. Clone this project into the docker container

`cd /tmp/ && git clone https://github.com/atakhq/tak-cert-enrollment-script.git`


3. Make the script executable and run it (we are inside the docker container)

`cd /tmp/tak-cert-enrollment-script/ && chmod +x * && ./certEnrollSetupScript.sh`


When prompted to move files around, answer 'y'

`Do you want me to move files around so that future server and client certificates are signed by this new CA? [y/n]`

Follow the prompts during the install to finsih up.
