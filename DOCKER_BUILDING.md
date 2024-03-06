
```bash
docker build -t eball/k3s-build -f Dockerfile.dapper .
docker run --rm -it --network host -v ${PWD}:/go/src/github.com/rancher/k3s/ eball/k3s-build build-k3s
```