## Recording a video with a Raspberry Pi and Camera Module

- With the camera connected, the following code will record 5 seconds of video footage and save it as `test.mp4` in the folder where your python script is saved.

```python
from picamzero import Camera

cam = Camera()
cam.start_preview()
cam.record_video("test.mp4", duration=5)
```

- By changing the number of seconds within `duration=5`, longer or shorter video clips can be played.
