Info about this fork
===

This fork introduces some improvements to the original project. See the list below.

What is done:
---

1. Gury object now can have "initialize(gury)" method which is called immediately after it was added to the gury set.

2. Gury object now can have "testPosition(x, y)" method which is used by gury to detect if the point belongs to the object. Performance boost.

3. Gury object's "update()" method now is passed the following arguments:
    - gury (Gury instance)
    - time (milliseconds from the beginning of the animation)
    - delta (current frame duration)
    - count (current frame number)

	All this data is calculated for the current object (i.e. if it was paused for example).

4. Gury's "play(interval)" method now has default argument. Default is 14 ms (i.e. up to 72 FPS).

5. Bug fixed: remove object's event handlers when removing object.