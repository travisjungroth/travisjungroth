---
title: "Workplace Education"
---
# Workplace Education
**I'm not persuing this idea as a product right now.** You can see what I'm working on on the [homepage](/).
## Description
### Problem
Getting everyone at a company to know something is really slow and expensive. People generally don’t know the right thing much of the time. Much more detail [below](#more-thoughts).
### Possible Solutions
Knowledge deployment software. Have everyone at your company know the things they should. It'll include a [spaced repetition](https://en.wikipedia.org/wiki/Spaced_repetition) component.

## Evaluation
The scorecards below are explained [here](/scorecards-explained).
### Problem
|  Metric   | Terrible | Bad        | Good        | Great        |
| --------- | ------ | ------------ | --------- | ----------- |
| Popular   | <10k   | >10k         | >100k     | ✔️>1m         |
| Growing   | <0%    | >0%          | ✔️>10%      | >20%         |
| Urgent    | >Year  | <Year        | <Month    | ✔️Right now   |
| Expensive | <$10m  | >$10m        | >$100m    | ✔️$1b+        |
| Mandatory | Averse | Nice to have | ✔️Important | Law changed |
| Frequent  | Yearly | Monthly      | Weekly    | ✔️Hourly      |

### Insight
|   Metric    |            | Won't have | Can have | Have |
| ----------- | ---------- | ---------- | -------- | ---- |
| Founders    | 1 in 10    |      ✔️      |          |      |
| Market      | 20%/year   |            |     ✔️     |      |
| Product     | 10x better |            |     ✔️     |      |
| Acquisition | $0         |      ✔️      |          |      |
| Monopoly    | Yes        |      ✔️      |          |      |

### Additional
#### Who desperately needs this product?
Companies with large workforces that change procedures frequently.

#### Am I the target user, know them extremely well, or neither?
I know the target user well (so neither).

#### Is this designed and created to grow very quickly?
Yes.

## More Thoughts
One mental model that’s useful for office work is to consider that at the root of everything a worker does is information. Nearly all tasks are based on information, not physical abilities. A worker can be considered to have two parts: the internal and the external. 

The internal is their body and mind. There is not much to be done directly to the body. The mind is where they operate from. 

The external is all the resources they have available to them. The worker must have the knowledge that these resources exist and the knowledge of how to use them.

The only information that a worker has available to them all of the time is what’s in their mind. For all external information, they must know that it exists and how to find it.

“Workplace education” is the act of updating information, specifically what’s in the mind of workers. To use programming terms, you can create, read or update (deletion is [not yet possible](https://www.youtube.com/watch?v=rb9a00bXf-U)).
External information is what they have available to them.

- Documentation
- Recordings of meetings
- Old emails
- Saved chats
- Information in the minds of others

Inside their mind are two types of information

- Actual information
- Where to find information

When someone is met with a demand for information (most likely “what is the correct action here”) they may:

- Know the information
- Know where to find the information
- Know where to find the information about where to find the information (or an even longer chain)

All of these also have failure modes

- Know the wrong information
- Not know the information
- Not know where to find the information about where to find the information
- Not know that a demand for information has even occurred

There are two demands placed on the worker: recognize a demand for information has occurred and have a path to the information available to them.

But what about group work? Collaboration? All knowledge work is inherently individual. No one has direct access to the mind of the other. All we can do is influence their mind by affecting their experience (writing, talking, expressions) and allow our experience to be altered by them (reading, listening, looking).

Workplace attempts to change internal information have much room for improvement. They attempt to create information that isn’t needed. They don’t provide information when it is needed. They fail to notify about updates in external information.

- Workers need less internal information than they're given
- Reference invalidation is usually more useful than updates. I don’t need to know the new information, I just need to know that the old information is wrong and where to find the new information
- Information that needs to be internalized often isn't
    - Think of your last company email with a piece of information everyone “needs to know”. A week later, what percentage of employees could answer that information on a test? Either the update operation failed and there were damages or it wasn’t needed in the first place
- Information updates could happen in batches and with less interruption
- Demands for information could happen with less interruption
- Important information updates need to happen with much higher confidence

Shallow vs. deep work.

- Little must be in-mind
- Things that are in-mind require repetition and testing
- Information chains must be kept updated
- It is expensive to have other people’s minds in information chains
- Little must be updated immediately

A similar model is to compare a person to a computer. A human brain is more powerful than the most powerful super computer in raw calculations, though they're better at different things. One place where computers are wildly better is in code deployment; it's a solved problem. It can a litte annoying some times, and there are extreme cases (cosmic rays) but you people can reliably get instructions onto a computer and be confident they won't change over time. 

This is not at all true of humans. It's normal to transmit instructions to a person and only 20% of the information gets across. Can you imagine deploying a code change and only 20% makes it? The only reason humans can function at all is because of their incredibly powerful brains and all the other instructions they have to draw from (but maybe these aren't the instructions you want).

Even once the instructions are received, they're not stable. People forget. Or worse, misremember. It's only through reuse that the instructions get cemented.

I think there's a lot to be learned in comparing existing workplace education to code deployment. What would "continuous deployment for people" look like? What would happen if McDonald's could update their staff as fast as their servers? What does each component translate to (staging servers, testing, etc) in a person? I have some ideas.

If you'd like to talk about this idea, email me at [jungroth@gmail.com](mailto:jungroth@gmail.com) or put a time for a video call on [my calendar](https://calendly.com/travisjungroth/chat).
