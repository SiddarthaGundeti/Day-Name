# Day-Name

Input: Monday  16

Output: Tuesday

Question Explanation:

You are given the weekday of the first day of the month and a positive integer N. Your task is to determine the day of the week for the Nth day of that month. To do this, you need to consider the calendar for that month and calculate the day of the week.

For example, if the first day of the month is Monday and N is 16, you need to find out which day of the week falls on the 16th day of the month.

Logical Approach:

Let's solve this problem in three steps:

Step 1: Assigning weekdays to day numbers

To make the calculation easier, we'll assign numbers from 0 to 6 based on the day of the week. For example, if the input is "Sunday," we'll assign day = 0; if it's "Monday," day = 1, and so on up to "Saturday" with day = 6.

Step 2: Calculate the day number of the desired date

Suppose you want to find the weekday of the 17th of June, and you know that the 1st of June is a Tuesday.

How many days is the 17th of June ahead of the 1st of June? It is 16 days ahead, i.e., N - 1.
Add the day number of the 1st of June (Tuesday) to N - 1 to get the target day number.
 
To find the final day number of the target date, take the remainder when dividing by 7, as day numbers are from 0 to 6.

For example, if the target_day is calculated as 4, it represents Thursday.

Step 3: Convert the day number back to a weekday and print

Now, convert the day number back to the corresponding weekday and print it.

By following these logical steps, you can determine the day of the week for the given Nth day of the month based on the provided first-day weekday.
