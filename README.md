Docker build

docker build  -t qemu_yocto  --build-arg username=yocto  .     

Docker Run

docker run -it  --rm --name=yocto_container --ipc=host --user=$UID --volume $(pwd):/home/yocto -w /home/yocto qemu_yocto