[![Build Status](https://travis-ci.org/agoda-com/adb-butler.svg?branch=master)](https://travis-ci.org/agoda-com/adb-butler)
[![Docker Stars](https://img.shields.io/docker/stars/agoda-com/adb-butler.svg)]()
[![Docker Pulls](https://img.shields.io/docker/pulls/agoda-com/adb-butler.svg)]()

# adb-butler
adb-butler is one of the components of [android-farm](https://github.com/agoda-com/android-farm) that runs adb server as a side-car container in kubernetes deployment of OpenSTF providers.

# Features
- self-healing
  - reconnect devices missing in adb server by rebinding the usb driver
  - reconnect devices missing or unstable in OpenSTF by restarting the adb connection
- clean-up rethinkdb for temporary emulators that are no longer available
- adding notes to provided devices
- automatic installation of test-butler for emulators
