# px4-docker-camera-sim

## STEPS

### Install docker 
```
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
```

### (Optional) Install nvidia container runtime
Installing this will allow for rendering of simulations with the dedicated nvidia graphics card if present, speeding up simulations by a large factor.
Follow the guide here https://developer.nvidia.com/nvidia-container-runtime

### Build docker image
Clone this repository and build the docker image
```
git clone git@github.com:basmango/px4-docker-camera-sim.git
cd landing-sim
sudo bash build_image.sh
```

### Launching containers
In the repo directory, run either of the following commands.
```
sudo bash launch_sim_nvidia.sh # if graphics card is present and nvidia runtime is installed as mentioned previously
sudo bash launch_sim.sh # launches simulation with integrated graphics card

```
