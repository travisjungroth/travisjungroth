---
title: "Creating Test Data"
---
# Creating Test Data
I made a prototype of this idea and a [video](https://www.loom.com/share/8e7be6d899bd498ea7e9325812a9d459).
## Description
### Problem
Creating test data for manual QA is hard. Creating test data for an external test system ([Rainforest QA](https://rainforestqa.com), Selenium as a separate service) is even harder. People who write test plans often aren't able to code. Much more detail [below](#more-thoughts).
### Possible Solutions
A database transaction recorder. Turn it on, create one example of the data that you want, then have an option to multiply. This will all get saved as executable SQL, so a new test database can be created instantly. No coding required, but the outputs are changeable.

## Evaluation
The scorecards below are explained [here](/scorecards-explained).
### Problem
|  Metric   | Terrible | Bad        | Good        | Great        |
| --------- | ------ | ------------ | --------- | ----------- |
| Popular   | <10k   | ✔️>10k         | >100k     | >1m         |
| Growing   | <0%    | >0%          | ✔️>10%      | >20%         |
| Urgent    | >Year  | <Year        | <Month    | ✔️Right now   |
| Expensive | <$10m  | ✔️>$10m       | >$100m    | $1b+        |
| Mandatory | Averse | Nice to have | ✔️Important | Law changed |
| Frequent  | Yearly | Monthly      | ✔️Weekly    | Hourly      |

### Insight
|   Metric    |            | Won't have | Can have | Have |
| ----------- | ---------- | ---------- | -------- | ---- |
| Founders    | 1 in 10    |     ✔️       |          |      |
| Market      | 20%/year   |      ✔️      |          |      |
| Product     | 10x better |            |      ✔️    |      |
| Acquisition | $0         |      ✔️      |          |      |
| Monopoly    | Yes        |            |     ✔️     |      |

### Additional
#### Who desperately needs this product?
Manual QA engineers, people using automated testing services.

#### Am I the target user, know them extremely well, or neither?
I know the target user extrememly well. I was a solutions engineer selling a crowd testing product for a year.

#### Is this designed and created to grow very quickly?
Yes.

## More Thoughts
I worked at [Rainforest QA](https://rainforestqa.com) as a Solutions Engineer, but the more accurate title was Sales Engineer. For seven months I was exclusively on sales calls (I’d later spend another seven months with customers). Getting a proper testing environment set up was a concern on every deal. Usually we worked through it, and about 20% of the time it killed the deal. If it didn’t kill it outright, it could be a contributing factor.

There are three parts to having a testing environment: having the environment infrastructure (app servers and databases), handling external services and creating test data. I don’t think there’s a current business opportunity in making the infrastructure easier to set up. That’s PaaS + the company internals.

Setting up external services for a test environment could maybe be a business. By “external” I mean software from other companies that the team relies on. Mocking is a lot of work and non-programmers can’t do it. Making mock APIs for other companies that don’t have great ones would be useful to someone. It would also be a huge amount of horizontal work. Reminds me of Zapier.

Creating test data is what I’m most interested in of the three. 

There are a few levels of difficulty for creating test data. Creating test data is pretty easy for programmers. They just write code to create the test data in the testing scripts. And, even if that problem is hard, I don’t think it’s solved by a business. It’s solved by better testing libraries.

Creating test data for manual QA engineers is harder. Creating simple cases is easy, maybe even easier than for programmers. They just use the app. Creating things in higher numbers is harder. They can’t just do a for-loop and create a hundred user accounts. Managing test data is even harder yet. Whereas the most common practice in test databases for automated tests is just to wipe the database and recreate it each test cycle, manual QA engineers don’t do this. It takes them longer to create the data (a minute vs a millisecond) so they keep it around. After any test, they’ll go back and manually reset the changes they made or create a new instance.

Creating test data for external automated testing is hardest of all. There isn’t backdoor code running to set up the data like in a local testing script. And there isn’t a manual QA engineer to get things just right. Even if there’s a set up a script that runs before the testing suite kicks off, there’s no pairing of the test data with each individual test. Some of these external testing solutions also promise that non-testers can write tests. This falls apart if they can’t set up the data.

I think there’s a real problem here, in a growing market. I have a vague idea of a solution: record the database activity of an app manually being set up for testing, then replay those transactions. To work, it would have to require no coding and be easy to set up. I also think it would be helpful if the data creation scripts were hackable, but this isn’t the essential part.

I have a few big open questions. How do you isolate the activity of a tester so people can record/test at the same time? Will this work with microservices?

If you'd like to talk about this idea, email me at [jungroth@gmail.com](mailto:jungroth@gmail.com) or put a time for a video call on [my calendar](https://calendly.com/travisjungroth/30min).
