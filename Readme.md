docker pull tensorflow/tensorflow:latest-gpu-jupyter

add 'DOCKER_OPTS="--dns 8.8.8.8"' to /etc/default/docker

docker run -u $(id -u):$(id -g) -v $(pwd):/tf/mnist_tutorial -p 8888:8888 tensorflow/tensorflow:latest-gpu-jupyter