# k8s-demo

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
  
### Kubernetes
- Update the `deployment.yaml` file in containers category with image repository url
`image: <dockerhub-username>/k8s-demo:1.0`
- Create the deployment.
`kubectl create -f <filename>.yaml`
- Check the deployment and the pods
`kubectl get deploy,po`
- Expose the deployment to the internet via loadbalancer
`kubectl expose deployment nodejs-deployment --type="LoadBalancer"`
- Check the service
`kubectl get svc`

🎉🎉 You have successfully deployed your container image to Kubernetes!!
