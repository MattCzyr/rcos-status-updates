## Last Week's Accomplishments
Last week I wrote code to fetch the vehicles, stops, and updates from
shuttles.rpi.edu and initialize them into arrays. For routes and stops, which
won't change often, I wrote code to cache the fetched data to JSON files so it
won't get fetched every time the app opens. I also found a bug where the HTTP
request to fetch the data was asynchronous, so the arrays were never being
populated with the fetched data. I was able to fix it by making the request
synchronous. I also did a lot of refactoring, making sure all the backend code
follows the same conventions and documenting methods using Swift-flavored
Markdown.

## This Week's Plan
My goal for this week, while the frontend is being worked on, is to figure out
which way each shuttle arrow should be facing based on the change between
updates.

## Anything Blocking?
N/A

