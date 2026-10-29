CPA CE – TI-84 Plus CE Program
==============================

Version Information
-------------------

This is version 1.0. This document was last edited 2025-06-19. And was created 2025-06-19.

Description
-----------
CPA-CE is a TI-84 Plus CE program designed to compute the Closest Point of Approach (CPA) between two vessels at sea. It uses a relative motion model based on vector trigonometry, assuming constant speeds and courses for both vessels. The program helps maritime navigators assess risk of collision and make informed decisions based on predicted separation distance and timing.

The program assumes your own ship's course is 000° (true north). The contact's course is entered as a true bearing. This simplifies input and makes calculations consistent with standard maneuvering board principles.

The user provides the own ship's speed and heading-relative bearing and range to a contact, along with the contact's course and speed. The program calculates:

- CPA distance (in nautical miles)
- Time to CPA (in minutes)
- Relative bearing to the CPA position (signed, in degrees)

Variables Used
--------------
| Variable | Description                                      | Units         |
|----------|--------------------------------------------------|---------------|
| S        | Own ship's speed                                 | Knots         |
| B        | Bearing to contact (relative, signed ±180°)      | Degrees       |
| R        | Range to contact                                  | Nautical miles|
| C        | Contact's course (true)                          | Degrees       |
| V        | Contact's speed                                  | Knots         |
| D        | CPA distance                                     | Nautical miles|
| T        | Time to CPA                                      | Minutes       |
| A        | Relative bearing to CPA position                 | Degrees       |

How to Use the Program
----------------------
Once the program is running:

- Enter your own ship’s speed in knots.
- Enter the bearing to the contact (signed relative bearing in degrees, from -180° to +180°).
- Enter the range to the contact in nautical miles.
- Enter the contact’s true course in degrees.
- Enter the contact’s speed in knots.

The program will display:

- CPA distance (nautical miles)
- Bearing to CPA (signed relative bearing in degrees)
- Time to CPA (minutes)

Example
-------
Own ship speed: 10 knots  
Bearing to contact: -45° (port bow)  
Range to contact: 6.0 nm  
Contact course: 135°  
Contact speed: 15 knots

The program returns:

CPA = 1.831 nm  
CPA Bearing = -117°  
Time to CPA = 14.79 min

This means that the contact will pass closest to your vessel at 1.831 nautical miles, on the port quarter, in approximately 14.79 minutes.

Notes
-----
- Assumes constant course and speed for both vessels.
- Own ship's course is always assumed to be 000°.
- Bearings must be entered as signed relative bearings.
- Final CPA bearing is output in signed format (±180°) relative to your ship’s heading.
- Program clears all working variables upon completion.
