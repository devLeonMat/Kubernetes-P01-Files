### Kubernetes-P01-Files


#### generate new image
```bash
docker build -t {repository name}:{tag version(1.0)} {route file (.)}
# Example:
docker build -t helloworld:1.0 .
```

#### add tag name
```bash
docker tag {current tag} {new tag}
# Example:
docker tag helloworld:1.0 helloworld:latest
```

#### view metadata
```bash
docker inspect {image id | image name}
```

#### create container
```bash
docker create {image id | image name}
docker create --name {container name} {image name}
docker create -p {host port:container port} --name {container name} {image name}
```

#### Delete container
```bash
docker rm {image id | image name}
docker rm {image id | image name} -f

```