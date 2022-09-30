# 101 Pool Game Case Study
---

### Objectitve: 
Maximize Revenue and Increase User Engagement by optimizing Configuration(Entry Fee - Seats - Composition) Parameters.

### Limitation: 
In order to optimize parameters, one should have a balanced approach rather than gravitating weightage to one end. Also Cut% (Revenue Parameter) can not be changed drastically.

### Based on the EDA done using Python Profiling. Here are some findings:

> Entry Fee: Most Common Values are: 25 (11.4%), 100 (11.2%), 1000 (11.2%) 10 (10.6%) and 50 (10.6%)

> Seat : 6 is around 80.4% while 2 is around 19.6%
 
> Composition: 2 is most common with (36.7%) while 6 is least common (14%), 3 is 16.8%, 4 is 16.4% and 5 is 16%
 
> Cut %: .15 is most common with 61.7% followed by 0.1 with 24.5%
  
> Rake: Most common is 1800 with 1.2% followed by 360 which is 1%
 
> Wager: Most common is 3000 which is 1.2% followed by 6000 which is 1.1%

### Key Findings after EDA

[EDA](https://github.com/probablyvivek/Rummy/blob/main/pandas_profiling.html) was done using Pandas Profiling library.


1. Average Revenue Generated per Month
![Month](https://github.com/probablyvivek/Rummy/blob/main/Average%20Revenue%20Generated%20per%20Month.png?raw=true)

Most profitable month is September while least is January.

2. Average Revenue Generated per Weekday

![Weekday](https://github.com/probablyvivek/Rummy/blob/main/Average%20Revenue%20Generated%20per%20Weekday.png?raw=true)

Most profitable day is Wednesday while the lease profitable day is Friday.

3. Average Revenue Generated per Composition

![Composition](https://github.com/probablyvivek/Rummy/blob/main/Average%20Revenue%20Generated%20per%20Composition.png?raw=true)

In terms of average revenue generated, Composition 3 is the most profitable while Composition 6 is the least profitable.

4. Average Number of User Cash Game Count per composition

![User Cash Game Count](https://github.com/probablyvivek/Rummy/blob/main/Average%20Number%20of%20User%20Cash%20Game%20Count%20per%20Composition.png?raw=true)

In  terms of Users Cash Game Count, Composition 3 and 4 have the highest numbers.

5. Average Number of Users per composition
![Users](https://github.com/probablyvivek/Rummy/blob/main/Average%20Number%20of%20Users%20per%20Composition.png?raw=true)

In terms of Users, Composition 3 and 4 have the highest numbers.

6. Average Revenue Generated per Entry Fee

![Entry Fee](https://github.com/probablyvivek/Rummy/blob/main/Entry%20Fee%20vs%20Revenue.png?raw=true)

Based on the data, we can make 10 Entry Fee as the default starting option as 5 Entry Fee is creating the least revenue.

Entry Fee 2500 can also be removed as the number of users either choose 2000 or 3000 as Entry Fee when it comes to choosing in that range.

We can also remove Entry Fee 25 as Entry 50 is generating almost same number of users and revenue as Entry Fee 25.

So, based on the above numbers we can think of keeping the following Entry Fee options:
    
    1. 10
    2. 50
    3. 100
    4. 250
    5. 500
    6. 1000
    7. 2000
    8. 3000
    9. 5000
    10. 10000 






