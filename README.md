# R and Jupyter
Simple Jupyter Notebook with R running in docker

## Prereqs
* Install [Java](https://java.com/en/download/manual.jsp)
* Install [Docker Desktop](https://www.docker.com/products/docker-desktop)
** Note, if you are installing on Windows, Docker Desktop requires Windows 10 pro.  Support for Windows 10 home is coming [soon](https://www.docker.com/blog/docker-desktop-for-windows-home-is-here/)

## Getting Started
### on Windows
I haven't tested these steps...

1. Clone the repo
2. cd into `jupyter-r`
3. run `gradlew.bat build` to build the docker image.  this will take a few min
4. run `gradlew.bat run` to start a container from the image, and open a web browser to the jupyter application.   If the page comes up saying it can't connect, wait a minute to see if it opens.
If you close your browser for any reason, run ```gradlew.bat open``` to open the a
pp in browser again.

Any changes you make will be saved to your local filesystem.

Run `gradlew.bat stop` to stop the running container.

### on Mac
1. Clone the repo
2. cd into `jupyter-r`
3. run `./gradlew build` to build the docker image.  this will take a few min
4. run `gradlew run` to start a container from the image and open a web browser to the jupyter application.  If the page comes up saying it can't connect, wait a minute to see if it opens.

If you close your browser for any reason, run ```./gradlew open``` to open the app in browser again.

Any changes you make will be saved to your local filesystem.

Run `./gradlew stop` to stop the running container.

## Updating the environment

## Is this really the best tool for R notebooks?
* Perhaps [R Notebooks](https://minimaxir.com/2017/06/r-notebooks/) are better than Jupyter Notebooks for R.
* Perhaps you don't need to manage docker locally and instead can use [Binder](https://mybinder.org/)
