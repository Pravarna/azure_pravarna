# Todo list

The frontend code is written in React and uses an environment variable file `.env` that holds the secrets. Since `.env` file holds the secrets, it has not been pushed to the repository.

The Azure resources you will work with are Azure App Services and ACR.

Your tasks are to:
1. Deploy an Azure App services webapp onto an appropriate App service plan.

2. Setup a build pipeline that pushes the frontend app docker image to ACR
    
    * The Dockerfile already exists in the `docker` folder
    
    * Make sure NOT to overwrite the existing docker images in the ACR
    
    * You will need to figure out a secure way to include the `.env` file in the Docker image

3. Setup a release pipeline to deploy the newly built image to the Azure App service.

4. Automate the build and deployment process to trigger on push or merge to the main branch of the git repository.

5. Point the web app to a custom domain and secure it with HTTPS. (SSL Certificate)

5. Update the `README` with the pipeline build status and the latest version of the docker image


## Misc

The contents of the `.env` file are as follows

        OC_API_BEARER_TOKEN=xxxxxxxxxxxxxx
        OC_API_URL=https://platform.onecircle.in/api/