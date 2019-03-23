## Last Week's Accomplishments
Last week I worked on improving the shuttle prediction algorithm that I wrote
earlier. Before, the shuttle predictions didn't cause the markers on the map to
move properly because of a few bugs, including:
- The code to determine how many seconds elapsed since the last update was
  received didn't take into account that update times are in UTC
- The last received update's closest point index wasn't being set properly
- Calculating the distance between points in the route incorrectly

These issues have now been fixed and we're closer to having working shuttle
predictions.


## This Week's Plan
This week I plan to complete the first attempt at shuttle prediction so that we
can run some tests on its performance and determine what we can do to make it
more accurate. At the moment, it seems that the predicted locations will
typically be a bit further ahead of the actual locations.

## Anything Blocking?
N/A

