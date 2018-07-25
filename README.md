# Doing a Sync Shift

## Starting Your Shift
When you start your shift:

- Open up the [Expert Chat](https://learn.co/expert-chat) window
- Write `qbot in sync` in the `#technical-coaches` Slack channel
- Greet the other TCs on shift and see how the day has been going 

## During Your Shift
While on sync, you'll wait to be queued for a screenshare. `qbot` will message you on Slack with the questions details if you've been queued by the dispatcher. You can then start a Zoom meeting and send the student a Zoom invite link. When you greet them, you can `@mention` them when you introduce yourself. That way they get a notification if they have chat minimized, for example: "Hey @cassaram09! you can join me here! https://zoom/2343252" (not a real link).

If you are free, you will need to go through the inactive questions and mark any questions with a response of 10 hours or older resolved. Make sure to type to them something like: "Hello! It looks like this question has been inactive for over 10 hours and will be resolved. If you still need help please open a new question. We’ll be more than happy to help! Thanks!". They will recieve an email with that last response, so if they are looking for their chat, they know why it was resolved.

If all the older inactive questions have been resolved and you still are free, feel free to help dispatch out. Pick a question from the chat, click the clipboard at the top as if you were going to queue up a question (see above image). Paste into `#technical-coaches` channel, replace `queue` with `take`. The format should look like `qbot take <link>`. That will assign the question to you. Then you can help them in chat and ask if they would like to pair program. If you take a question make sure to ask them: "Would you like to pair program for 20 minutes?".

## Before the Screenshare
Please be sure to familiarize yourself with the [screen share documentation](https://github.com/flatiron-labs/learn-support/blob/master/screen-sharing.md) **UPDATE THIS**.

Each pairing session should be limited to 20 minutes (We recommend blocking out 15min for the pairing itself, and 5min for the setup time). After you greet the student, if they do not reply to you in 5 minutes, you will want to mark them unresponsive by typing in `qbot unresponsive`. This will place the question on hold for 5 minutes before assigning the question to the next available TC. If you are the TC that gets assigned an unresponsive question, message the student on AAQ to see if they are ready to continue. If they have still not replied since the last link was given, you can do `qbot unresponsive`. If you notice the question is older than 30 minutes with no response from the student, then you can `qbot done` the question in order to resolve it.

## During the Screenshare
While pairing with the student, you should use _annotations_ and the _clock_ on Zoom. Annotations are great for focusing the student's attention on certain parts of the code without having to control their screen. *Note: if the student has their current window in full screen mode, they may not be able to see annotations.* The clock displays how much time has elapsed since you joined the meeting, which is helpful for sticking to the 20 minute mark. [Follow these instructions to enable the clock](https://support.zoom.us/hc/en-us/articles/115002542683-Show-My-Connected-Time-in-a-Meeting). 

Working within a time limit can be difficult and you won't be able to solve all problems in 20 minutes. That's OK. If you notice you're starting to come up on time, then try to leave the student with some next steps / action plan (e.g. "Try putting a pry here.", "Look into what the variable index equals in this method." "Take another look at this lesson on Rails Routes."...) and let them know if they still need a hand that they can hop back in the rotation for another pairing.

If you feel the student needs more help (e.g. you were unable to find out what the issue was), let the student know that you are out of time and would like a fresh pair of eyes to view their issue. Ask them if they would like to be placed back in the queue. Most students appreciate this and don't mind being added back to the queue. To add them, you can type `qbot more help` in the `#technical-coaches` channel. After they've been added, let the student know they're in the queue.

Be sure to keep an eye on your pairing time and in the `#technical-coaches` channel for any notices from dispatch alerting you you're close to time. You can send a DM in Flatiron Staff to `qbot` using `qbot who is on?` to see how long you have been pair programming. If you're around 18 minutes, start to wrap up with the student. If they still need help, `qbot more help` and follow the guidelines described above.

## After the Screenshare
If you feel the student's issue has been resolved, you can resolve the question you have with `qbot done`. It's also nice to leave them with a farewell in the chat after you wrap up screenshare, and remind them to resolve the chat (we should *not* resolve the question for them).

## Student Cannot / Will Not Screenshare
Occassionally, students will not be able to pair program or will prefer not to. If possible, try and find some way to synchronously work with the student, even if it's just 1 on 1 in the chat. We want to give them some meaningful time with our full attention to help them for those 20 minutes.

If they have a bad internet connection, you can do chat only support (no Zoom). Have them `learn save` so their latest code is pushed to Github. Once they have pushed their code, you can get the url from clicking on the Github link near their profile information:

![github link](https://s3.amazonaws.com/learn-experts/expert-chat-github-link.png)

This will take you to their forked repository and you can get the url to clone their repo. This will allow you to debug with the student and see all of their errors locally.

## Ending Your Shift
If you recieve a question 5 minutes prior to the end of your shift, you can `qbot more help` it to the next available TC. If you recieve a question 2 minutes prior to the end of your shift, you will need to `qbot more help` and then `qbot out`. Any questions assigned to you for 2 minutes or longer will need to be added back to the queue before you `qbot out`.

If you run out of time with a student and you're not at a good stopping point, you can let them know that you're happy to put them back in the queue and have another coach come on to help them in a minute. After ending your share, `qbot more help` in Slack and the question will be automatically reassigned.

If you're not on with a student, you can simply `qbot out` to end your shift.

## Resources

* [Screen Share Documentation](https://github.com/flatiron-labs/learn-support/blob/master/screen-sharing.md) **UPDATE THIS**
* [Qbot Commands](https://github.com/flatiron-labs/online-ed-ops/blob/master/technical-coach-team/role-technical-coach/lib/qbot.md) 
