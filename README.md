# iterative-grabcut: Using simple rectangle for identifying foreground items

This algorithm is uses a rectangle made by the user to identify the foreground item. Then, the user can edit to add or remove objects to the foreground. Once done, it removes the background and makes it transparent (adds alpha channel) and saves it.

This is a simple notebook implementing the [GrabCut algorithm](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_grabcut/py_grabcut.html) shown in the [High-Quality Background Removal Without Green Screens | State of the Art Approach Explained](https://youtu.be/rUo0wuVyefU) video on What's AI's channel.

## How does it work? With example

1. Upload your image.
2. Create a rectangle over your image including all your foreground objects.
3. Remove the background using GrabCut algorithm.
4. If improvement is needed, draw on the image, left click (white) = foreground and right click(black) = background.
5. Remove the background using GrabCut algorithm.
6. Return to step 4 or end.

## Video demos

### Example with one iteration to correct the first pass of the algorithm:

https://user-images.githubusercontent.com/70274208/115054227-00367880-9eae-11eb-8281-320c5fa658f1.mp4


### Example with harder picture and multiple iterations:

https://user-images.githubusercontent.com/70274208/115054217-fca2f180-9ead-11eb-8777-373596f75165.mp4

## Results:
<p float="left">
  <img src="https://user-images.githubusercontent.com/70274208/115054345-21976480-9eae-11eb-9074-75edd6f448f2.jpg" width="300" />
  <img src="https://user-images.githubusercontent.com/70274208/115054258-09bfe080-9eae-11eb-8561-0027fed61450.png" width="300" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/70274208/115054347-222ffb00-9eae-11eb-896c-52459acd1997.jpg" width="300" />
  <img src="https://user-images.githubusercontent.com/70274208/115054260-0a587700-9eae-11eb-933c-54057090eab0.png" width="300" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/70274208/115054351-222ffb00-9eae-11eb-894c-545beaa357f2.jpg" width="300" />
  <img src="https://user-images.githubusercontent.com/70274208/115054254-09274a00-9eae-11eb-8b5b-fbe16cb59311.png" width="300" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/70274208/115054354-22c89180-9eae-11eb-9405-293ae17dc131.jpg" width="300" />
  <img src="https://user-images.githubusercontent.com/70274208/115054256-09bfe080-9eae-11eb-8172-770839512cb3.png" width="300" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/70274208/115054349-222ffb00-9eae-11eb-904b-1331d767c61a.jpg" width="300" />
  <img src="https://user-images.githubusercontent.com/70274208/115054262-0a587700-9eae-11eb-9c8c-1bbdab60ad38.png" width="300" />
</p>


References:

Interactive Foreground Extraction using GrabCut Algorithm, OpenCV, (2013), https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_grabcut/py_grabcut.html
