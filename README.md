# docker_usage

reference link
  - 전반적인 사용 방법
    : https://greeksharifa.github.io/references/2021/06/21/Docker/
  
  - docker image for pytorch
    : https://hub.docker.com/r/pytorch/pytorch/tags
    
  - nvidia container toolkit
    : https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html
  
  - docker shared mem 늘리는 법
    : --shm-size=8G
    
  - GPU 모두 사용
    : --gpus all
    
  - 메모리 문제 해결
    : --ipc=host
  
  ----------------------------------------
  docker run -it --gpus all --shm-size=8G --ipc=host -p 6006:6006 --name torch_ex2 pytorch/pytorch:1.10.0-cuda11.3-cudnn8-devel /bin/bash
  
  docker run -it --gpus all --mount type=bind,source=/home/haksoo/Project/2023/EXACODE/_docker_mounted,target=/workspace/LocalMounted --name cd_pet rishubi/codegeex:latest /bin/bash

    
    
