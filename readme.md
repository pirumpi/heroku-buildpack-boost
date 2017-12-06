# Heroku Buildpack: Boost (for C++)

Installs the Boost C++ libraries

Download and compile boost for later buildpacks.

Python buildpacks on heroku like dlib use boost.  dlib fails if the findboost function fails.  This buildpack will download, complile, install and set the necessary hint environment vars for later python buildback to consume.  This allows dlib to compile successfully.

## Usage

Designed to be used with [`heroku-buildpack-multi`](https://github.com/heroku/heroku-buildpack-multi).

There will be strict warnings during output. Tested successfully with Python 3.6.3 and dlib 19.7.0.

