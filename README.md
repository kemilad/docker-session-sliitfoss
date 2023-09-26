# docker-session-sliitfoss-bashaway

## Commands  
### Node app
- Run the application locally.
`node index.js`

### Docker

- Docker build
`docker build -t sliit-bashaway .`
- Create and Run the Container
`docker run -p 3000:3000 sliit-bashaway:v1`
- Upload the image to Docker Registry - DockerHub
  - Tag the image
  `docker tag sliit-bashaway:v1 <dockerhub-username>/sliit-bashaway:v1`
  - Push it to DockerHub
  `docker push <dockerhub-username>/sliit-bashaway:v1`
  
🎉🎉 You have successfully deployed and pushed your container image to DockerHub!!
