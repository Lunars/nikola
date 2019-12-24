<p align="center">
  <img src="https://firebasestorage.googleapis.com/v0/b/nikola-ffeaf.appspot.com/o/logonovo.svg?alt=media&token=0370731f-6240-41bb-bb30-db1db4947655" height="80"><br><br>
  <a href="https://github.com/geraldoramos/nikola/issues"><img src=https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat></a> <a href="https://github.com/geraldoramos/nikola/releases/latest"><img src=https://img.shields.io/github/downloads/geraldoramos/nikola/total.svg?style=flat></a>
  <p align="center"><strong>⚡Unofficial cross-platform desktop app to monitor and control Tesla vehicles, powered by Electron & React</strong><p>
<img src="https://firebasestorage.googleapis.com/v0/b/nikola-ffeaf.appspot.com/o/bg1.png?alt=media&token=f2bbad8d-bd75-4b94-9134-a523f8278e24">

## Get Nikola

> Currently available for MacOS, Windows and Linux.

Download [last release](https://github.com/Lunars/nikola/releases/latest)

## Features

* Real-time location tracking
* Track of several statuses (Speed, battery, temperature, etc...)
* Remote locking/unlocking
* Remote climate control
* Remote sentry mode toggle
* Remote temperature target set
* Auto-update (of the app, not the car)
* Custom images for all Tesla models
* Dynamic icon for battery level
* Tesla AuthKey stored locally


## Contributing

Check work backlog [here](https://github.com/geraldoramos/nikola/projects)

You can generate the binary in the `packed` folder using:

```bash
# Dev
TESLAJS_SERVER=http://localhost:7654/ VIN=123 TESLAJS_LOG=2 GOOGLE_MAPS=123 yarn dev

# Build for prod
TESLAJS_SERVER=http://localhost:7654/ VIN=123 GOOGLE_MAPS=123 yarn build
```

To get port 7654 exposed from your car, you can use a port forward:

```bash
# Get nonStandardPort from your lunars/config.sh file
# 7654 is the car API
ssh -o StrictHostKeyChecking=no -L 7654:localhost:7654 root@yourserver.com -p $nonStandardPort ssh -L 7654:localhost:7654 root@localhost -p $nonStandardPort
```

## Todo

Check [Projects](https://github.com/geraldoramos/nikola/projects) for details.
