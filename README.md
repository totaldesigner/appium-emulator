Appium Emulator
===============

Appium server to run tests on Android emulators.

Images have been created based on Selenium images: https://github.com/rgonalo/docker-appium

How to use this image
---------------------

#### Launch the image

``` bash
$ docker run -d -P -p 4444:4444 --name appium-emulator totaldesigner/appium-emulator
```

#### Get Appium server ip and port

You can acquire the port that the Appium server is exposed to by running:


#### Run Appium tests

Execute your Appium tests on the remote server *192.168.99.100:49412*. The test will be executed in a Nexus 5 emulator
with Android 6.0 (API 23).

You can tail Appium server logs with the following docker command:

``` bash
$ docker logs --follow appium-emulator
```
