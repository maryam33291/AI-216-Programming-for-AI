Electricity Billing Problem

In this problem, we had to take the number of electricity units from the user and decide which billing category it belongs to (Basic, Standard, or High Usage).

.Logic Used

First, I took input from the user.

If units were less than or equal to 100 → Basic Rate.

If units were between 101 and 300 → Standard Rate.

If units were above 300 → High Usage Rate.

I used if-elif-else so that only one category is selected.

.Challenges Faced

At first, I forgot to convert input into integer.

input() gives string, so comparison with numbers caused an error.

I had to fix the condition order properly.

.Attendance Problem

We had a list of attendance percentages.
We needed to count how many students are allowed (75% or more) and how many are not allowed.

🔹 Logic Used

I created two counters: allowed and not_allowed.

I used a loop to check each attendance value.

If attendance was 75 or more, I increased the allowed counter.

Otherwise, I increased the not_allowed counter.

🔹 Challenges Faced

I mistakenly wrote =+1 instead of +=1.

I forgot to initialize counters to 0 at first.

That caused wrong output.

.Scholarship Problem

We had to check which students are eligible for a scholarship.
Conditions were:

CGPA ≥ 3.5

Family income ≤ 80000

🔹 Logic Used

There were two lists: CGPA and family income.

I compared values at the same index.

If both conditions were true, I increased the scholarship counter.

🔹 Challenges Faced

Initially, I compared the list name instead of individual values.

I used nested loops which created wrong combinations.

I also had a small print syntax error.

.Sensor Monitoring Problem

We had sensor readings and needed to find values outside the safe range (20–80).
Then count total alerts and calculate the percentage of alerts.

🔹 Logic Used

I used a loop to check each reading.

If reading was less than 20 or greater than 80, I increased the alert counter.

Then I calculated percentage using:

(alerts / total readings) * 100

🔹 Challenges Faced

Defining the safe range correctly.

Making sure percentage formula was correct.

Understanding that division gives float result.