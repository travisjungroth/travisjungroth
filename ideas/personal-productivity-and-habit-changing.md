---
title: "Personal Productivity and Habit Changing"
---
# Personal Productivity and Habit Changing
**I'm not persuing this idea as a product right now. You can see what I'm working on on the [homepage](/).** I'm going to just keep working on this one for myself.
## Description
### Problem
I've hacked together a system for productivity, learning and habit change using Todoist, Airtable, Zapier and Anki. I like it more than any off-the-shelf solution, which is weird. Much more detail [below](#more-thoughts).
### Possible Solutions
Basecamp for personal productivity and habit changing. Also using a spaced repetition component on habits.

## Evaluation
The scorecards below are explained [here](/scorecards-explained).
### Problem
|  Metric   | Terrible | Bad        | Good        | Great        |
| --------- | ------ | ------------ | --------- | ----------- |
| Popular   | <10k   | >10k         | >100k     | ✔️>1m         |
| Growing   | <0%    | >0%          | ✔️>10%      | >20%         |
| Urgent    | >Year  | ✔️<Year        | <Month    | Right now   |
| Expensive | <$10m  | >$10m        | ✔️>$100m    | $1b+        |
| Mandatory | Averse | Nice to have | ✔️Important | Law changed |
| Frequent  | Yearly | Monthly      | Weekly    | ✔️Hourly      |

### Insight
|   Metric    |            | Won't have | Can have | Have |
| ----------- | ---------- | ---------- | -------- | ---- |
| Founders    | 1 in 10    |     ✔️       |          |      |
| Market      | 20%/year   |     ✔️       |          |      |
| Product     | 10x better |            |     ✔️     |      |
| Acquisition | $0         |            |     ✔️     |      |
| Monopoly    | Yes        |     ✔️       |          |      |

### Additional
#### Who desperately needs this product?
People who really want self-improvement.

#### Am I the target user, know them extremely well, or neither?
I'm the target user.

#### Is this designed and created to grow very quickly?
Yes.

## More Thoughts
I cobbled together a system for tracking tasks and habits, and it has had a huge effect on my productivity. I think of it in three levels.

First is the meta-system. It’s how I make sure the system is working. I’m doing weekly reviews and writing things down. It’s similar to the idea of [Reflection](/ideas/reflection), but there’s nothing groundbreaking here.

Second is the system itself. The tasks component of this is pretty standard. I’m just using Google Calendar and Todoist. The habit part is what’s special. I added in Python and Airtable. I was using Zapier, but I’m not right now. More detail on this in a bit.

Third are the tasks and habits. Nothing too special here. Meditation, weightlifting and reading. I’m also using Anki, which made me realize my memory of books I read was essentially zero. I think there’d be a business in selling Anki (or other SRS software) decks of books if it wasn’t for all the copyright.

I didn’t use off-the-shelf habit tracking software because I didn’t see anything that fit. The main requirement I couldn’t find was I wanted my habits to be in task system, and I didn’t see one that handled both really well.

The system is pretty simple. I have a “habit” project in Todoist. In it are recurring tasks. I also have a Python script with the tasks. The tasks are duplicated, but I may rewrite it to pull from the Todoist API. Each week I run the script, which creates a list of the habits/tasks I want to do each day. It exports it in a tab separated format that I can paste into Airtable. At the end of each day, I mark off in Airtable which tasks I completed. I was doing this with Zapier, but I was hitting an API limit on Todoist with only a handful of requests. In Airtable, I’m able to see stats and a calendar related to my habits.

I’d love to have this all in one system. The tasks and habit tracking especially, but maybe some of the meta system and the habits as well. 

If you'd like to talk about this idea, email me at [jungroth@gmail.com](mailto:jungroth@gmail.com) or put a time for a video call on [my calendar](https://calendly.com/travisjungroth/30min).
