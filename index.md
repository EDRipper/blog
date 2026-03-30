# So you have users, now what?

Hack Club developers are uniquely privileged in their position. When launching a product we do not have to look far to our audience, we already have huge email lists and outreach. We do not have to seek out financial backing, every idea has an uncapped budget provided it runs with scalable economics. This makes Hack Club an incredible place to be building in, but it also creates a common hitch that at some point you will run into. You deploy something amazing, put it out there, get all the attention and then think "Great! Now what?".

Aside from the very real technical problems of scaling and increased load, a sudden influx of users engaging can provide just as many challenges as acquiring them in the first place does. I'm not the strongest backend engineer, so I want to use this blog to instead cover how I solved these part social and part technical problems that come with users, speaking on both learnings from failure and advice from success.


# #1 - If you haven't tried it, it doesn't work;
This seems obvious, but my biggest takeaway from developing platforms at scale is that every edge case will be found, and every situation tested. If you haven't tested a process yourself, assume it doesn't work. It's always going to be easier for the user to leave and never look back than for them to find the support channel and make a ticket, so it isn't safe to assume you would hear about it if it's a real issue. An example of this is with Campfire Flagship, where brand new users were added to the flagship Slack channels but never the #Welcome-To-Hack-Club channel. This left 246 users partially onboarded to the Slack, and they all left silently, because with no prior context or investment, why would they bother finding the bug report flow?

Similarly I took for granted the Hack Club office WiFi, and it took months for anyone to realize that anybody on 3G had to wait 10 seconds for the site to load. Realistically all of those potential users just clicked away forever, they had no motivation to wait or let me know.

Test the unhappy case, never assume. Try it on incognito, on patchy mobile data, on an obscure browser with a strange screen ratio. If you haven't tried it, it doesn't work.


# #2 - Nothing is self-sustaining;
You could have the perfect onboarding scenario, you could have tons of guides and an active Slack channel, but energy naturally dissipates. Keeping a system at the same level of usage requires constant energy input. I think of this like entropy, In terms of physics, there are many more non useful arrangements of energy than useful ones, so given time any concentration of useful energy tends to dissipate into a 'random' arrangement. Similarly, keeping highly engaged users concentrated on one platform goes against their natural tendency, hence a platform will never fully sustain itself. If you architect a platform and don't engage with it, the users will leave. You need to be a part of the community yourself. 

Below is a graph showing the daily activity (in shipped projects) for Summer Of Making. Each spike represents a very intentional effort to drive engagement, but the general trend without effort is a downward slope. 

![A Graph of summer of making 2025 engagement over time](https://cdn.hackclub.com/019d1d97-30e9-76be-a185-ba56dda1f0e3/image.png)


So how do I keep users shipping? Lock-in huddles
 are a great way to build a sense of community, but it only works on a small scale. The biggest issue is the barrier to entry, joining a huddle is an act of participation that requires volunteering yourself to be social. The perfect approach puts everybody in a collaborative situation with an achievable but high stakes goal, without them having to volunteer themselves. I believe we pulled this off effectively in Summer of Making, and the prolonged graph spiked in mid August backs this up. 

The idea for SOM was simple - the event would end and the website would be sunk if not enough people shipped projects. The artificial pressure got highly invested users to start, which we helped along with lock in huddles, but then as the task was a collaborative goal they started asking their friends to help out;

![img](https://cdn.hackclub.com/019d3d50-d602-7ab1-8a2d-5449f5364854/image.png)
- 
The artificial urgency was backed by an elaborate lore post about Heidi and Orpheus hoisting the summer of making island to safety with balloons. For sure the premise was absurd, but we (not least staff) embraced the game in full, sharing our struggles as we tried to send every shipper a balloon as a thank you. I remember hanging out on a livestream until stupid O-Clock at HQ packing envelopes, only to discover 1 label had been double printed and have to re-scan every envelope to find it.

![img](https://cdn.hackclub.com/019d3d5e-fca8-77e4-8ca0-2f7636d7db2a/image.png)



# #3 - How to be kind x1000
It's very easy to be personable and responsive to a small, intimate community where you can remember each person and the context around their progress. When you have thousands of users at different stages, you cannot feasibly be on top of each problem as it occurs, so the real problem becomes one of min-maxing for 3 variables, effort, scale and effectiveness in how you communicate.
An effective communication is targeted, but a targeted communication is effort. 
A scaled communication means a blanket approach that can be very low effort, but is often not effective.
Identifying large groups that could all benefit from the same small nudge is a real hack to keeping people engaged.

When running CFFS we polled every user for their intention. This was first applied as a scaled communication, we sent the simple question do you want to come to the hackathon to a huge audience.
The results allowed us to make more targeted approaches, atomising our users into groups of
- No concerns - already engaged, leave them alone
- Needs a push - interested but not on track
- Wants to come but can't qualify - a different problem entirely
- Doesn't want to come - don't waste their inbox

 For the least effort, the highest yielding group to target was those who need a nudge, I was then able to write a template email and send it to this group while seeming like I was emailing them individually.


![an email prompting the user to reach out for any help needed](https://cdn.hackclub.com/019d3cbd-5edc-7588-8a86-c46059c847ce/image.png)

And again, by grouping our users into atomised distinct categories we were able to see exactly the shift this made within our user funnel. 

When it came to finalising the attendee count I also opted to DM users with an automated Slack user token, rather than sending a channel wide ping, again coming across as available and personal. In reality my availability was limited, but people want the perception and comfort of on hand support more than they need the actual support. A direct message had a much greater response than an untargeted ping.


![a Slack DM asking if the user is attending](https://cdn.hackclub.com/019d3d6c-7ced-798c-b9ac-58e75b282979/image.png)

The underlying message here is that **eyes on the page are not the same as users, and users are not the same as participants.** Once you've got attention, your job is to move people down that chain, and you can't do that with a blanket approach. Filter your audience as granularly as you can, be intentional about where you spend effort, and always ask what you're actually getting out of each communication. A message that sounds personal at scale is the winning ticket to good conversion. Getting this part right can be the difference between launching a platform and building a community.






