# TensorFlow-1.14.0-GPU installation on AWS

## Clone TensorFlowOnAWS repository.

```sh
cd ~

git clone https://github.com/look4pritam/TensorFlowOnAWS.git

cd /home/ubuntu/TensorFlowOnAWS
```

## Install NVIDIA driver.

```sh
./ubuntu-18.04/install_nvidia_driver
```

### Verify NVIDIA driver installation.

```sh
nvidia-smi
```

## Install CUDA-10.0.

```sh
./ubuntu-18.04/install_cuda-10.0
```

### Verify CUDA-10.0 installation.

```sh
nvcc -V
```

## Install Python3.

```sh
./ubuntu-18.04/install_python3
```

## Install TensorFlow-1.14.0-GPU.

```sh
./ubuntu-18.04/install_tensorflow-1.14.0
```

## AWS - Mount instance store.

### Check drives - nvme0n1 entry.
```sh
lsblk
```

### Mount instance store.
```sh
./aws/mount_instance_store
```

