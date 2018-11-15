# cuda

根據這個Dockerfile build image之後
透過以下指令產生container
$nvidia-docker run  -it -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix -v $HOME/.Xauthority:/root/.Xauthority --net=host -P --device /dev/snd  --name tmp amostsai/cuda:latest
