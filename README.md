#Keras-1.2-with-TensorFlow-and-MXNet

To use jupyter notebooks open a powershell and apply the following steps:

1. Make sure DOcker is installed, running and that your drive is shared in docker settings.
2. Navigate to your project working space
3. `docker run -it -v ${PWD}:/tmp/working -w=/tmp/working -p 8888:8888 --rm [image name] jupyter notebook
--ip="*" --notebook-dir=/tmp/working --allow-root`
You can find the image name with the command: `docker images`

