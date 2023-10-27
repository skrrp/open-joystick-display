# Open Joystick Display
**A powerful and easy to use streamer-ready overlay for your joystick or gamepad. Completely free and open source.**

### Project Discontinued

This project has been discontinued. I no longer have time or money to support this product due to recent events in my life. Links below to the archived source and last compiled binaries. You can find archived documentation listed below as well. This project was open source, so if someone wants to fork and make a new version by all means do so. As of writing the application works just fine from my testing except for one documented bug regarding the N64 RetroSpy configuration.

## Build artefacts
The link in the parent repo that was here for downloading the build artefacts is long-dead and is now being domain-squatted by a scummy online pharmacy. As such, it is impossible to download pre-built binaries any more.

I have forked the repo and added the `/build` directory. It contains a `Dockerfile` and a build script. You DO NOT need to check out the whole repo to make a build, but you may do so if you wish.

### Build instructions in 2023
* Install `docker`
* Download the 2 files in the `/build` directory or navigate to it if you have done a full checkout
* Ensure that `build.sh` is executable
* Run it: `./build.sh`
* Docker will do its thing and when it has finished there will be a new `dist` directory in `/build` directory. This contains the build artefacts

I will note that building this application in 2023 throws up some fairly scary warnings. Since I am not an Electron developer I can't say how dangerous this all is. If anyone wishes to keep the code up to date I will accept PRs on this fork. I have used this fork in the build process as I note the parent is archived.

If you are not a developer and are only using `docker` for this one thing, you may need to clear up some base images to reclaim disk space.

    $ docker image ls
    REPOSITORY                      TAG                   IMAGE ID       CREATED          SIZE
    node                            12-bullseye           bafd2af2faeb   18 months ago    917MB
    
    $ docker image rm -f bafd2af2faeb

Replace the image ID in the last command with the one you get from your `docker image ls` command.

## Documentation

### License
https://github.com/KernelZechs/open-joystick-display/blob/master/LICENSE.md

### Changelog
https://github.com/KernelZechs/open-joystick-display/blob/master/docs/changelog.md

### Development and Deployment Guide
https://github.com/KernelZechs/open-joystick-display/blob/master/docs/build.md

### Getting Started
https://github.com/KernelZechs/open-joystick-display/blob/master/docs/getting-started.md

### Theme Development
https://github.com/KernelZechs/open-joystick-display/blob/master/docs/theme-development.md
