# shift-worker-rate-calculator-excel
A simple Fortnightly Pay Calculator spreadsheet for Microsoft Excel I created about 10 years ago for working in a petrol station, I've slightly generalised. and made public.

## What it includes:
* 14 days to add a start time, finish time, and time on (unpaid) break
* Pay scaling based oan age
* An expenses list that can be expanded 
* A bunch of hard-coded formulas that are a pain in the neck to maintain.
* A quick payment percentage calculator to assist with budgeting
* Automatic calculation of taxation for Australia, FY2022 by extracting data from [The Withholding Lookup Tool Available Here](https://www.ato.gov.au/Rates/Fortnightly-tax-table/)

## What it assumes:
* Pay rate is calculated by _start time_
* You are paid fortnightly
* Pay rate is set for the entire shift, not per hour
* You are claiming the Tax-Free Threshold

## What it doesn't include:
* Localised content for any other regions than Australia
* Modify access to Taxation functions.
** The ATO "protected" this by hiding functional lookup rows, and "protecting" the sheet with a password. This was bypassed, but reinstated for this sheet.
* Superannuation functions
* Annual leave calculations
* Calculation of HECS debts or other mandatory Australian Government repayments
* Calculation of any other mandatory Government payments (i.e. Child Support)
* Any consideration for your actual 

## How to enter Start and Finish Times:
Enter start and finish times as _decimal_ hours in _24-hour notation_
For example: 
* 8am --> 8
* 9:30pm --> 21.5
* 12:15am --> 0.25

## How to enter Break Durations:
Add up all unpaid breaks, and use _decimal_ hour durations.
For example:
* 2x Paid 10-minute breaks + 1x 30-minute unpaid break --> 0.5
* 1x 1-hour unpaid break, + 1x 30-minute unpaid break --> 1.5

## What if my pay week is calculated based on shifts from Saturday to Friday instead of Monday to Sunday?
Just change the weekday names. Weekday names are not utilised in any other calculations.
