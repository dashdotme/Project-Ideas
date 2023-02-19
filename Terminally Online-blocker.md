# Terminally Online-blocker
Auto-mute people who post above a given frequency.

Applicable for:
- reddit <-- MVP
- twitter
- forums


### Core idea:
Start with a JS script which parses a page 
- for each user on page
	- calc post frequency in last month (via [API](https://www.reddit.com/dev/api/))
	- if freq > X (eg. 10 posts per day):
		- block user, set flag
	- if freq > Y (where Y < X):
		- lookup kindness (via [user-analyser](https://reddit-user-analyser.netlify.app))
		- if kindness < Z:
			- block user, set flag
- if flag
	- reload page 


### Then:
Make this configurable 
- optionally block based on kindness only
- maintain 'blocked' list
	- context in blocked list (map username to subreddit they were blocked from)
		- can highlight negative subs
- 'unblock all' function (maintains list)
- 'purge list' function (unblocks and empties list)
- 'update' function (reruns checks on users in list)


### Delivery: Chromium extension
ie. add a manifest, import to edge/chrome and test

Publish if it's useful and works. 


### Extensions
Extend for twitter, forums (Github, hackernews)



