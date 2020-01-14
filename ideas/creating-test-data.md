---
title: "Creating Test Data"
---
# Creating Test Data
## Description
### Problem
Creating test data for manual QA is hard. Creating test data for an external test system ([Rainforest QA](https://rainforestqa.com), Selenium as a separate service) is even harder. People who write test plans often aren't able to code.
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
Manual QA engineers, people using testing service.

#### Am I the target user, know them extremely well, or neither?
I know the target user extrememly well. I was a solutions engineer selling a crowd testing product for a year.

#### Is this designed and created to grow very quickly?
Yes.
