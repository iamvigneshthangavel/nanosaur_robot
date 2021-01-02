# nanosaur

NanoSaur is a little tracked robot ROS2 enabled, made for an NVIDIA Jetson Nano

## Install
```
mkdir -p dev_ws/src
cd dev_ws/src 
```

## Build Docker

```
docker build -t nanosaur .
```

### Run docker container

https://answers.ros.org/question/358453/ros2-docker-multiple-hosts/

```
docker run --net=host --device /dev/i2c-1 -it --rm nanosaur
```

## Docker Compose

Install Docker compose on jetson-nano

```
sudo apt-get install -y libffi-dev
sudo apt-get install -y python-openssl
sudo apt-get install libssl-dev

pip3 install -U docker-compose
```
