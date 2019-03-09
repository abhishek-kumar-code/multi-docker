# multi-docker
Building a multi-container (React, Express, Postgres, Redis) component application with a nginx routing server to run a Fibonacci Calculator

Multi Container Setup Flow
- Push code to GitHub
- Travis automatically pulls repo
- Travis builds a test image, tests code
- Travis builds prod images
- Travis pushes built prod images to Docker Hub
- Travis pushes project to AWS EB
- EB pulls images from Docker Hub, deploys 
