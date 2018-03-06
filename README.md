#Keras-1.2-MXNet

Using this dockerfile you can build the image from scratch yourself, alternatively you can also find a [pre-built image from my docker repository here](https://cloud.docker.com/swarm/rickvm/repository/docker/rickvm/keras-mxnet/general)


Build the image
If you want to build the image then copy the dockerfile to a directory of choice, open a powershell there and execute:
`docker build . -t [name:tag]`
So for example:
`docker build . -t [Keras-mxnet:latest]`


Run image and use jupyter notebooks open a powershell and apply the following steps:

1. Make sure Docker is installed, running and that your drive is shared in docker settings.
2. Navigate to your project working space
3. `docker run -it -v ${PWD}:/tmp/working -w=/tmp/working -p 8888:8888 --rm [image name] jupyter notebook
--ip="*" --notebook-dir=/tmp/working --allow-root`
You can find the image name with the command: `docker images`

