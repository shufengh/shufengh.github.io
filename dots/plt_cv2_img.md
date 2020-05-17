Use mapplotlib to show images opened with OpenCV2
===

OpenCV represents images with dimensions of BGR instead of regular RGB as expectd by matplot

```python
import matplotlib.pyplot as plt
import cv2

image = cv2.imread("test.jpg")
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
```

@cv
