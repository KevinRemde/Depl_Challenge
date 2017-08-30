# The Deployment Challenge

## The goal:
This this lab, your assignment is to create and deploy a containerized app.

## The steps:

### Get the croc-hunter repo
You'll find it [HERE](http://github.com/kevinremde/Depl_Challenge).

### Compile and run the app locally

You already have a provided Dockerfile, so what is the command to build (hint hint) the image?

And do you remember how to run it and connect to it on your local computer?

## Push the container to a container registry

If you don't have one, you'll want to set up your own free registry on [hub.docker.com](http://hub.docker.com).  

Hint: You'll need to **tag** your image to match the registry name / image before you **push** it.

### Create a web app (Linux Preview) in Azure and configure it to pull your app container

Did you know that you can connect/associate a linux-based container to/with an Azure Web App?  Try it out. Set it up to pull your croc-hunter container from your Docker hub registry. _Bonus kudos for you if you configure your app to refresh when a newer version of the container is put in your Docker hub registry._

### And then try this...

Change the croc-hunter.go file, line 44, to run "game2.js".  Re-build and re-push your container, and see if the boat starts shooting fish instead of laserbeams.  

## Extra Credit

### Here are some things you can try to take this to the next level:

1. Install Kubernetes on ACS (Note: look for instructions online to it from the CLI)
2. Install [Helm](https://helm.sh/) locally (Note: You'll have to find a way to get the 2.5.1 version specifically.  There is a bug in Tiller on ACS that keeps it from upgrading properly, and local Helm and server Tiller version have to match. )
3. Search Helm for a useful app solution to install. (you can search from the command-line, or use the [Kube App site](https://kubeapps.com/).
4. Use Helm to install it.
5. Use Helm to install Jenkins, and see if you can get a full CI/CI build automation to work better than Kevin could. 



# More info on Croc Hunter - The game!

For those that have dreamt to hunt crocs

# Usage
Basic go webserver to demonstrate example CI/CD pipeline using Kubernetes 

# Deploy using Jenkins Chart and Helm
[![Demo Pipeline](https://img.youtube.com/vi/NVoln4HdZOY/0.jpg)](https://youtu.be/NVoln4HdZOY "Demo Pipeline")

# How to setup the Jenkins infrastructure 
[![Jenkins Setup](https://img.youtube.com/vi/eMOzF_xAm7w/0.jpg)](https://youtu.be/eMOzF_xAm7w "Jenkins Setup")
* See DEMO.md for steps
