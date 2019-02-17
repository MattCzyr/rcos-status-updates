## Last Week's Accomplishments
Last week, I finished the backend work on notifications and began working on
the frontend for the Settings panel and the Schedule panel.

On the backend, I...
- Created a Trip struct to store the starting point, destination, time to get
  on the shuttle, and arrival time. This allows notifications to be triggered
  easier.
- Set nearby notifications to only trigger once every 60 seconds for each route
  ID.
- Let notifications trigger even when the app is in the foreground. This will
  be especially useful for nearby notifications.


On the frontend, I...
- Created the Settings and Schedule storyboard scenes. The Settings scene
  contains sliders to show/hide shuttle routes, enable/disable nearby
  notifications, and will include a field to schedule "trips" to be notified for.

## This Week's Plan
This week, I plan to;
- Fix an issue that I have been assigned to in which some updates contain
  unknown key/value pairs.
- Fill in the rest of the options in the Settings scene.
- Merge all my notifications and Settings work into master. There will be some
  overlap with other frontend work that has been done in the meantime, so I will
  have to fix this as well.

## Anything Blocking?
The only blockers I encountered this week were related to how storyboards work,
but I was able to figure them out.