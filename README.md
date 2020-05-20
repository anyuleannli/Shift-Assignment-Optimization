# Shift-Assignment-Optimization

Trevon is in charge of scheduling shifts for all 50 nurses at the emergency department at Trojan community hospital. In order to help the hospital retain quality staff, Trevon would like to create schedules that treat all nurses fairly and satisfy their preferences as much as possible. In the past, he spent many painstaking hours scheduling by hand, but he feels that the schedules can still be improved. Recently, Trevon learned about mixed-integer programming (MIP) in a course he is taking at USC. He would like to apply his knowledge to create better schedules for the nurses.

The shifts are scheduled n weeks at a time (beginning on a Sunday and ending on a Satur- day). (n is a parameter that can be inferred from the input data.)

Shift requirements: There are three nurse shifts in a day: morning, evening, and nights. Each shift should have exactly a certain number of nurses, which is specified in the input file.

Scheduling constraints: Based on hospital and union regulations, no nurse can be assigned more than 6 shifts in a calendar week (Sunday to Saturday). Moreover, no nurse may be sched- uled to consecutive shifts. In addition, if a nurse works in a night shift, he/she also cannot be assigned to either a morning or evening shift the day before or the day after the night shift.

Finally, each nurse can blackout a certain number of shifts, indicating times he/she cannot make (due to vacations and other conflicts). Blacking out a shift means that the nurse has a hard conflict and will not take that shift under any circumstances. Which shifts are blacked out for each nurse can be inferred from the input file.

Nurse Preferences: For each shift, a nurse may indicate a preference score of 0, 1, or 2. A score of 0 indicates that the shift is blacked-out, and he/she cannot be assigned to it. A score of 1 indicates that the time is not preferred, but the nurse is willing to work if needed. A score of 2 indicates a preferred time slot.

Objective: Trevon would like to maximize the following objective, subject to satisfying all shift requirements scheduling constraints,
