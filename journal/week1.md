# Week 1 — App Containerization

## Class Summary
- [x] Create a new GitHub repo
For this case i created a new github branch in this repo
<image src="/images/branch.jpg" alt="branch">

- [x] Launch the repo within a Gitpod workspace
For start i using the button Gitpod on Github or start the workspace on Gitpod

First Gitpod Offline
<image src="/images/gitpoddown.jpg" alt="Offline">

Second Gitpod Online
<image src="/images/gitpodup.jpg" alt="Online">

- [x] Configure Gitpod.yml configuration, eg. I’m VSCode Extensions

For this case i edited the .gitpod.yml for using AWS and VS Code extensions
<image src="/images/vscode.jpg" alt="VS Code">

- [x] Clone the frontend and backend repo

I'm using the command
git clone https://github.com/cmq008/aws-bootcamp-cruddur-2023.git

- [x] Explore the codebases
In the exploration i have the response
<image src="/images/directory.jpg" alt="Directory">

- [x] Ensure we can get the apps running locally
First i need to install the requirements with this command
pip3 install -r requirements.txt

For local running i apply these commands
```sh
cd backend-flask
export FRONTEND_URL="*"
export BACKEND_URL="*"
python3 -m flask run --host=0.0.0.0 --port=4567
```
<image src="/images/localrunning.jpg" alt="Running">

To test the running i open the port 4567 and access with a browser, later i append the url /api/activities/home

<image src="/images/localrunproof.jpg" alt="Proof">

- [x] Write a Dockerfile for each app

Backend Dockerfile
<image src="/images/dockerbuild1.jpg" alt="backend">

Frontend Dockerfile
<image src="/images/dockerbuild2.jpg" alt="frontend">

Docker image ls
<image src="/images/dockerimagels.jpg" alt="List">

- [x] Ensure we get the apps running via individual container

First i launch the backend
<image src="/images/dockerrunback.jpg" alt="Backend">

Second i launch the frontend
<image src="/images/dockerrunfront.jpg" alt="Frontend">

For this case i'm using the command docker ps
<image src="/images/dockerps.jpg" alt="List">

- [x] Create a docker-compose file
<image src="/images/dockercompose.jpg" alt="Docker Compose">

- [x] Ensure we can orchestrate multiple containers to run side by side
Contenedores corriendo
<image src="/images/activeports.jpg" alt="Active Containers">

- [x] Mount directories so we can make changes while we code

Implementación de volúmenes
<image src="/images/volumes.jpg" alt="Volumenes">