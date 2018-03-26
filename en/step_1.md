## Recording a video with a Raspberry Pi and PiCamera

- With the camera connected the following code would record 15 seconds of video footage and save it as `my_video.h264`.

```python
from picamera import Picamera
camera = PiCamera()

camera.start_recording('my_video.h264')
camera.wait_recording(15)
camera.stop_recording()
```

- By changing the time number of seconds within `camera.wait_recording()`, longer or shorter video clips can be played.
