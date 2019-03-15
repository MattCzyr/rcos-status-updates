## Last Week's Accomplishments
Last week, I:
- Fixed issue #30 in which there were some unknown key/value pairs appearing
  when initializing Route objects. There were `active` and `schedule` keys
  added to the datafeed that we did not account for in the Route constructor's
  switch statements. While I was at it, I changed the debug messages for
  unknown key/value pairs to show where they're coming from. I opened a PR with
  these changes, which has been merged.
- Added a `closest_stop` variable to Points, which stores the closest Stop to
  the Point and is calculated when the Point is initialized.
- Made a first attempt at using my shuttle estimation algorithm to predict
  shuttle positions in between updates. Every second, the estimation algorithm
  is called on each active shuttle and used to update its marker on the map.
  Every 10th second, new updates are checked for, and if they are any they will
  be used to update the shuttle positions. This solution is not very accurate
  at the moment.

## This Week's Plan
This week, I plan to work on my shuttle prediction algorithm to make shuttle
position estimates more accurate. I'll also be trying to find a more elegant
solution to checking for new updates, rather than receiving them every 10 seconds
and seeing if they've changed since the last batch received. If I have extra
time, I may also work on making the settings panel look a bit better, as right
now some of the elements are not aligned properly.

## Anything Blocking?
N/A

