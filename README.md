# Calendar to take care of my grandmother
In 2022, I created this calendar because my aunts and uncles were having trouble creating a calendar for taking care my grandmother that was reliable and unbiased. For example, on 2023 my aunt made an uncle take care of my grandmother for 5 consecutive days because he 'magically' dropped on a group of dates that were holy week, plus weekend, plus a holiday.

This calendar generator tries to address this issue.

As an input, you have to provide:
- The list of care givers and an RGB color to identify them.
- The list of holidays for a given year. You may also want to add right now the first of January next year.
- The start date and amount of days you want to generate.

This algorithm works the following way:
- It assumes there is a paid caregiver taking care of my grandmother during working weekdays.
- A caregiver from the list will be assigned at least 1 day but no more than 3 days in a row.
- If there are more than 4 days in a row, it will switch the caregiver to the next one and split the 4 days into 2 for each caregiver.
- The caregivers will be assigned from the `care_givers` variable in a circular order.
- It does not take into account the possible vacations the paid caregiver would take off.

I had this code sitting down in [jupyter.org](https://jupyter.org) for around 2 years. But I finally decided to back it up here.

## Calendar for 2024
![Calendar for 2024](https://github.com/estuche77/grandma-caregiver-calendar-generator/blob/main/2024-calendar.png?raw=true)
