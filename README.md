****

# openapi2jsonschema docker image



## Usage



1) Clone this repo

2) Run this command (in the root directory) to build the images and run container in detached mode.

> `docker-compose up -d`

3)  Run this command to enter into the container 'bash' mode

> `docker-compose run python-openapi2jsonschema-bash bash`

4) Now you can run the [openapi2jsonschema](https://github.com/instrumenta/openapi2jsonschema) command to generate json schema files from swagger (openAPI) definition files. You can previously copy the input swagger files in the **swagger** directory of the repository (mounted as volume in the container)

> `openapi2jsonschema /tmp/swagger/petStore.json`