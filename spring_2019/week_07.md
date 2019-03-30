## Last Week's Accomplishments
Last week I fixed an issue in the shuttle prediction algorithm that caused
point indices in routes to go out of bounds. I also changed the way shuttle
markers are displayed on the map by just updating the coordinates of existing
shuttle annotations instead of removing all annotations and creating new ones
every time. I also stopped Points from keeping track of the closest stop since
this information won't be needed regularly.

## This Week's Plan
This week, I plan to finish reworking the way annotations are updated, as the
new approach does not totally work yet. I also plan on once and for all
finishing the first attempt at shuttle prediction and opening a PR with all the
changes I've made, as I did not get to do that last week.

## Anything Blocking?
Time was the only blocker I encountered this week due to a couple tests.

