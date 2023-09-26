# docker-session-sliitfoss

## Commands  
### Node app
- Run the application locally.
`node index.js`

### Docker

- Docker build
`docker build -t node-server .`
- Create and Run the Container
`docker run -p 3001:3001 node-server:latest`
- Upload the image to Docker Registry - DockerHub
  - Tag the image
  `docker tag node-server <dockerhub-username>/k8s-demo:1.0`
  - Push it to DockerHub
  `docker push <dockerhub-username>/k8s-demo:1.0`
  
🎉🎉 You have successfully deployed your container image to Kubernetes!!
