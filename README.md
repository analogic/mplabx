# mplabx

docker run -it --name mplabx \
    --privileged \
    -v /dev/bus/usb:/dev/bus/usb \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    -v /path/to/mplab/projects:/path/to/mplab/projects \
    -e DISPLAY=unix$DISPLAY \
    analogic/mplabx


xhost +