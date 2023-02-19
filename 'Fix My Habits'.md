# 'Fix My Habits'
Inject into webapps to provide a slightly worse experience. Idea here is to manipulate our wiring for those habits we want to kick (eg. social media).


### Actual implementation should
- add function, distorting the viewport slightly
	- this does a lot for discomfort, surprisingly
- add clock tracking time spent on page/in app
- provide a daily/weekly history for pages viewed
- optionally display other things you care about, eg. 
	- your 'hobby' list
	- your 'health' scores from a smartwatch etc.
	- upcoming entertainment you're looking forward to

Point here is to respect individual judgment. Give people the right information in a useful way and they'll do wiser things. 
- Social media often does the opposite


### Related ideas
https://one-sec.app/ 
- novel idea, great fix for mobile
- inconvenience and awareness seems better than time wasting
	- delaying page loads would be another simple 'fix', but mainly encourages removing the app...


### Possible simple ML extension:
- classify text content based on conflict
	- good = green = low score 
	- bad = red = high score
- display running score for viewed pages
	- by session 
	- in total

Applying classification to your own feed would be insightful, like viewing your kindness score on https://reddit-user-analyser.netlify.app/