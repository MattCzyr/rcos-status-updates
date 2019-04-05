## Last Week's Accomplishments
Last week, I:
- Realized that shuttle updates seem to be in KM/H and not MPH and fixed the
  shuttle estimation calculations accordingly.
- Finished changing the way annotations are updated. They are no longer removed
  and added back every second, which caused the shuttle markers to flash on the
  map, and instead the coordinates and headings are simply updated on each
  annotation. Annotations are refreshed (removed and added back) every
  5 minutes in order to remove expired annotations for shuttles that are no
  longer on the map.
- Made calculations (and then fixed those calculations) for shuttle headings in
  shuttle estimations.
- Split the `initUpdates()` function into `initUpdates()`, which now just
  initializes the updates from the datafeed and stores them, and
  `propagateUpdates()`, which sends each update to the respective shuttle.
- Refactored some code, mainly in the ViewController.
- Am currently in the process of opening a PR with shuttle prediction.

Commits:
- [9b2d564](https://github.com/quuu/iShuttleTracker/commit/9b2d564c0cc7dcc98c7c6e96cfbca71a0834e520)
- [cba702c](https://github.com/quuu/iShuttleTracker/commit/cba702c4fa634b9ec88df186d1fb01bada138acd)
- [a56d1b8](https://github.com/quuu/iShuttleTracker/commit/a56d1b8f9617ffa067dae3fb4e36cf9b99564ccc)
- [caf4ff7](https://github.com/quuu/iShuttleTracker/commit/caf4ff7c5a0a7469ce27cbc9421412776090b879)

## This Week's Plan
This week, I plan to get the shuttle prediction PR approved, merged, and
integrate the work I've done with the rest of the work that's been done
lately, specifically with the settings panel.

## Anything Blocking?
N/A
