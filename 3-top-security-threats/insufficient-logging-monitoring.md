# Insufficient Logging and Monitoring

If our app isn't being monitored by any tools or don't have insufficient logging mechanisms in place with alerts when something suspicious and our resources is being executed, how will we prevent cyber criminals from completely getting control of our app or pulling data from it?

## Senario 01

On average our site gets 200 users per day and we allowcated resources for that workload. Suddenly our app jumps to 500 users and then 1000 or more. How will we determin if this is official user growth or a cyber criminal trying to execute a Denial of Serevice (DoS) attack?

### Summary

1. Average 200 users per day.
2. Sudden spike thousands of users.
3. How will we know why the sudden surge?
4. How will we know when it happens?
5. Is it an attack or growth?

## Monitoring and logging

This is key to supervise our resources, user growth and cyber criminal trying to break into our app. Most host providers have tools for us to use for this purpose and we MUST use them well - set 'alerts' so we get notifications for unusual behaviors then make sure we set some type of user base monitoring and we can either use prebuilt resources such as Google Analytics, elastic search or build our own within our app. This will help us from getting caught from lost resources because a cyber criminal has exploited them.

### Summary of Monitoring & Logging

- Performance of servers.
- Server activity logs.
- User logs.
- Network logs.
- Google analytics.
- Appliation analytics.

1. Most host providers have these logs.
2. Use tools such as Google Analytics and ElasticSearch.
