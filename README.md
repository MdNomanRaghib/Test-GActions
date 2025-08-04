1. Took a demo Node.js application which simply gives the result "Welcome to DevOps !!".
2. Node.js application consists of index.js, package.json and Dockerfile in the repository.
3. github workflow is created.
4. main.yml file is set to "Trigger on push to main".
5. build-and-deploy job is configured which do code checkout, install Node.js, dependencies, build docker image and later on pushes the docker image to docker hub.
6. Secrets are created to login to docker (username and password) repository level which is used in main.yml file.
7. The created image can be deployed to a remote server like ec2 instance etc.
8. To deploy the web application we can create secrets like REMOTE_HOST, REMOTE_USER AND SSH_PRIVATE_KEY at repository level similar to what we did while docker login step in main.yml.
