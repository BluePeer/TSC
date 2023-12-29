[back](../../README.md)
# Basic stuff
You can find the video [here](https://www.youtube.com/watch?v=5bNX74AK3Yo)

In the video we showed which basic programs you should have on your computer in order to work as comfortably as possible.

## Video Steps

### yarn install after Node.js Installation
To make yarn available globally you have to add the -g parameter to the npm install, otherwise yarn will only end up in your local npm installation.

    npm install -g yarn

### Prepare and Install alt:V Server with altv-pkg

To download an alt:V server using altv-pkg. 
It is enough to execute the following command in the console.

    npx altv-pkg [branch]
    branches: release/dev/rc
    
If you want the whole thing in more detail.
You have to create the following file in the appropriate folder (where the server should be).
> Filename: **.altvpkgrc.json**

    {
	    "loadJSModule": true,
	    "loadBytecodeModule": false,
	    "loadCSharpModule": true,
	    "loadJSV2Module": false,
	    "loadVoiceServer": true
    }

### Setup altv-xts-boilerplate

#### Download

    git clone https://github.com/xxshady/altv-xts-boilerplate.git
#### Setup 

    yarn setup-project
#### Start
To build the js code and enable folding.

    yarn dev
To start the server choose one of the following variants (depending on the OS)
##### Windows
Run the included server-dev.bat, this starts the server with the settings from the server-dev.toml
or start the server manually

    altv-server.exe --config server-dev.toml

##### Linux
Make sure you have given execute rights to both the altv server and the altv crash handler.

    chmod +x altv-crash-handler
    chmod +x altv-server
then nothing stands in the way of starting

    ./altv-server  --config server-dev.toml

## Used Websites and Resources
- [x] [altv-xts-boilerplate](https://github.com/xxshady/altv-xts-boilerplate) by [xxshady](https://github.com/xxshady)
- [x] [alt:V Website](https://altv.mp/)
- [x] [alt:V Docs](https://docs.altv.mp/js/index.html)
- [x] [alt:V Hub](https://hub.altv.mp/)
- [x] [Forge](https://forge.plebmasters.de/) by [DurtyFree](https://github.com/DurtyFree)

## Download links

 - [Node.js LTS Version 20.XX.XX](https://nodejs.org/en/download/)
 - [Visual Studio Code](https://code.visualstudio.com/)
 - [git command line interface](https://git-scm.com/downloads)
