BUSPLAN-CE – TI-84 Plus CE Program
==================================

Description
-----------
BUSPLAN-CE is a TI-84 Plus CE program designed to help transit planners, schedulers, or trainees determine the number of buses required on a route to maintain a given headway. The program uses the total round trip time (T), a layover time expressed as a percentage (L), and the desired headway (H) to calculate the total cycle time and determine how many buses are needed to maintain the planned service frequency.

Variables Used
--------------
| Variable | Description                                      | Units       |
|----------|--------------------------------------------------|-------------|
| T        | Round trip time (driving time only)              | Minutes     |
| L        | Layover time as a percentage of T                | Percent (%) |
| H        | Headway (desired interval between buses)         | Minutes     |
| B        | Number of buses required (rounded to nearest 0.1)| Buses       |

How to Use the Program
----------------------
Once the program is running:

- Enter the round trip time (T) in minutes when prompted.
- Enter the layover time as a percentage of the round trip time (L).
- Enter the desired headway (H) in minutes.
- The program will calculate and display the number of buses required, rounded to the nearest 0.1 bus.
- Press [ENTER] to clear and exit.

Example
-------
A bus route takes 60 minutes to complete a round trip.
Planned layover time is 15% of the round trip.
You want a 10-minute headway between buses.

Run the program and input:

RTime= 60
LayOv= 15
HdWay= 10

You’ll see:

Buses=   6.9 req'd

Explanation:
Layover time is 15% of 60 → 9 minutes
Total cycle time = 60 + 9 = 69 minutes
69 ÷ 10 = 6.9 buses

Notes
-----
- The result is rounded to one decimal place, allowing for flexibility in planning.
- This program automatically clears variables when finished and resets the home screen.
