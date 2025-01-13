# Preparation

### Working PC

Prepare Linux-Based PC with the following packages installed.

- Docker

You can follow this guideline for installing Docker on your PC, with comprehensive instruction for each Linux's Distribution [this page](https://docs.docker.com/engine/install/).

### Install media

You can get the media by pulling this repository [this page](https://github.com/fadhilyori/me2-deploy.git)

## Media Preparation

Copy files to your preferenced directory. If you don't have the install media yet, see [this page](https://github.com/fadhilyori/me2-deploy.git)

## Setting up for Sensor

- Make sure you have already set the network configuration for your entire system.
- Open `docker-compose.sensor.yml` using text editor.
- Modify `MES_CLIENT_SERVER` value to your Defense Center's PC IP Address.
- Save the change.
- Open your terminal and run:

```
    docker compose -f docker-compose.sensor.yml up -d
```

- Wait until the process is done.
- You can check whether the services is running by typing:

```
    docker ps
```

- If the services already running, you can continue to set the defense center.

## Setting up for Defense Center

- Make sure `docker-compose.dc.yml` already exist.
- Open your terminal and run:

```
    docker compose -f docker-compose.dc.yml up -d
```

- Wait until the process is done. This process took longer time compared with creating sensor's container.
- You can check whether the services is running by typing:

```
    docker ps
```

- Open your browser and browse your localhost to enter into OpenDashboard.

```
    http://localhost:5601
```

## Adding More Sensor

If you want to add more sensor, you can redo [this step.](Installation-and-Configuration#setting-up-for-sensor)
