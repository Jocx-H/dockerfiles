### 构建容器

```shell
docker build -t sparta:118 .
```

### 启动容器

```shell
docker run --gpus all -it --name <your_container_name> -v <path/to/your_file>:/project/test sparta:118
```

### 在容器中编译Sparta
```shell
cd ../sparta

python3 setup.py install
```

### 注意

* 请尽量宿主机为CUDA 11.8及上的版本使用该Dockerfile构建
* 请在构建的时候联网