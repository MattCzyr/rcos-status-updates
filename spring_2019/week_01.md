## Last Week's Accomplishments
This week I worked on sending notifications for our app when shuttles are about
to arrive, so I spent a lot of time learning about local notifications and how
to use background refresh. It turns out that Apple does not allow apps to
consistently refresh data in the background, as we'd need for notifications in
this project. To work around this, I implemented two different notification
triggers:
- Time: Users will select what shuttle stop they need to get to, from where,
  and by when, and we will notify them when they should get on the shuttle.
- Nearby: When the app is in the foreground, we will notify the user when
  a shuttle on the selected route comes within a certain range.

These notifications are triggered by `tryNotifyTime()` and `tryNotifyNearby()`
in NotificationHandler, which are called whenever shuttle data is fetched.
To help with the time notifications, I also created a  Time class that gets the
time since the day began from a Date and has comparison operators.


## This Week's Plan
This week, I plan to:
- Finish the backend work for notifications. I plan on creating a struct to
  store the "trips" that the user needs to make, consisting of a starting stop,
  destination stop, and arrival time, so that notifications can be triggered
  more easily.
- Make a settings panel for the app through which you can choose when to
  receive notifications and toggle routes on and off.
- Make notifications display even when the app is in the foreground, as that
  is the only time nearby notifications will be received.


## Anything Blocking?
The only blocker I've run into so far was not being able to use background
refresh as I had hoped, but I think the workaround I found will work.

