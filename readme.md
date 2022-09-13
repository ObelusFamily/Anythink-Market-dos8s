<h1 align="center">Welcome to the Anythink Market repo</h1>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Contents
- [Installation](#installation)
- [Development](#development)
- [First setup](#first-setup)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## :floppy_disk: Installation
To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

#### :small_blue_diamond: Install Docker
:small_orange_diamond: For Linux, MacOS or Windows

  - Install Docker from [Docker](https://docs.docker.com/get-docker/)

:small_orange_diamond: For Arch Linux
  ```
  sudo pacman -S docker
  OR
  yay -S docker
  ```
   - Then install docker-compose package from AUR
  ```
  yay -S docker-compose
  ```

> :round_pushpin: _Note : Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md))._

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## :cloud: Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## :zap: First setup

<!-- 
  **[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_
-->

First of all, Let's Check if docker is properly installed.
- Run these commands to check docker version, if it prints the docker version then you are good to go :) , otherwise docker or docker-compose is not properly installed.
  ```
  docker -v
  docker-compose -v
  ```
Now, If you haven't already cloned the repo in your machine, Do it.
- Run this command to clone the repo
  ```
  git clone https://github.com/ObelusFamily/Anythink-Market-dos8s.git
  ```
After cloning the repo, cd into the repo (Go inside the folder named Anythink-Market-dos8s)
- Run this command to setup the local environment.
  ```
  docker-compose up
  ```
  > :round_pushpin: Note : In some Linux distributions, you might have to run it as super user
  ```
  sudo docker-compose up
  ```

If Docker is working correctly, the backend should be running and able to connect to your local database.
Let's test this by pointing your browser to - http://localhost:3000/api/ping

If this works then the backend is running, Now Let's check the frontend and make sure it’s connected to the backend.

Go to this address in your browser - http://localhost:3001/register .
If you were able to create a User on the page then Congratulations 🥳 You did it.

> Tip : Make sure that you run all scripts in the next quests on one of the containers created by ```docker-compose up```.  Also, you can use ```docker exec``` to run commands on a running container.

Now You can move on to the next tasks 👍.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
