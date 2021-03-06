x-gewinnt / connect-x
[![Build Status](https://travis-ci.org/fweidemann14/x-gewinnt.svg?branch=master)](https://travis-ci.org/fweidemann14/x-gewinnt)
[![codebeat badge](https://codebeat.co/badges/f7ef0129-b360-4eab-ad26-d761beb97dfc)](https://codebeat.co/projects/github-com-fweidemann14-x-gewinnt-master)
[![codecov](https://codecov.io/gh/fweidemann14/x-gewinnt/branch/master/graph/badge.svg)](https://codecov.io/gh/fweidemann14/x-gewinnt)
=====================

Description
-----------

`Python 3` recommended, not sure if it's mandatory though..

This repository contains a full and final implementation of the popular game `connect four` with a slight modification:
you may change the `four`!

Pre-Fun-Installations
---------------------
**IMPORTANT**:

__If you're not sure what you have installed on your system, you should do a `pip install requirements.txt` BEFORE doing any of the steps below! This will install all neccessary modules.__

*Also, I strongly recommend the use of `virtualenv`, specifically `virtualenvwrapper`. This will isolate the project path and allows you to install all dependencies in a virtual environment. After you're done you may delete your `venv` and your system is in the same state as before.*

If you just got curious and want to learn more about this, head over to the official [virtualenv documentation](https://virtualenv.pypa.io/en/stable/ "venv documentation") to get started.

Getting Started
---------------

There are serveral ways of starting this app.

`The simplest one` is rather boring. You'll just play the game in your `bash`.
That's it. No shiny interface. And you'll have to use your keyboard, obviously.
However, if that's the desired option, just `cd` into your cloned directory and type `python game/maintty.py`.
Now the game is starting up in your `bash` and you'll get hit with a small configuration screen. Follow the instructions and enjoy!

`The next option` is starting the game's web-service which allows you to play the game in your browser, look at an actual UI (not good though) and use your mouse to drop tokens. To do that, type `python webapp/webserviceguni.py`. This will start a `Gunicorn` WSGI Server on your localhost and listens on port `5001` for incoming connections.
Now navigate to your browser of choice (please no IE..) and type `localhost:5001`.

The last option is using Docker. You may use `docker-build -t your-image-name` inside the cloned repository to build a Docker image, or you can run `docker-compose up` to let it start up all by itself.

If you want to edit the source code, you may use the `webapp/webservice.py` as your primary development server. 

License
-------
GNU General Public License v3.0

Read more in the LICENSE.txt
