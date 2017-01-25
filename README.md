x11vnc-docker
====

Dockerfile for x11vnc with Xvfb.

Running
----

```bash
$docker run -it -p 5900:5900 -p 6099:6099 jumpeiarashi/x11vnc
```

Conneting display from another program
----

This container exposes X server tcp port. You can connect container virtual display with `DISPLAY` environment variables.

```bash
# in another machine
$DISPLAY=X11VNC_CONTAINER_HOST:99.0 xterm
```
