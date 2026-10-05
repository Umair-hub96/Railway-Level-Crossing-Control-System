# Task 3 — Identify Constraint Violations

## Violation 1 — C1

Constraint:
Train_Present → ¬Barrier_Open

Violation:
Train_Present = TRUE
Barrier_Open = TRUE

What went wrong:
The barrier is open while a train is present.

How do we know:
The constraint requires the barrier to be closed when a train is present.


## Violation 2 — C2

Constraint:
Train_Approaching → Barrier_Closed

Violation:
Train_Approaching = TRUE
Barrier_Closed = FALSE

What went wrong:
A train is approaching but the barrier is not closed.

How do we know:
The constraint requires the barrier to be closed when a train is approaching.


## Violation 3 — C3

Constraint:
Train_Approaching → Warning_Lights_On

Violation:
Train_Approaching = TRUE
Warning_Lights_On = FALSE

What went wrong:
A train is approaching but the warning lights are off.

How do we know:
The warning lights must be on when a train is approaching.


## Violation 4 — C4

Constraint:
Train_Approaching → Audible_Alarm_On

Violation:
Train_Approaching = TRUE
Audible_Alarm_On = FALSE

What went wrong:
A train is approaching but the audible alarm is off.

How do we know:
The audible alarm must be on when a train is approaching.


## Violation 5 — C5

Constraint:
Train_Passing → Barrier_Closed

Violation:
Train_Passing = TRUE
Barrier_Closed = FALSE

What went wrong:
The train is passing while the barrier is open.

How do we know:
The barrier must remain closed while the train is passing.


## Violation 6 — C6

Constraint:
¬Train_Present → Barrier_Open

Violation:
Train_Present = FALSE
Barrier_Open = FALSE

What went wrong:
No train is present but the barrier remains closed.

How do we know:
The formal constraint requires the barrier to be open when no train is present.


## Violation 7 — C7

Constraint:
Sensor_Failed → ¬Normal_Automatic_Operation

Violation:
Sensor_Failed = TRUE
Normal_Automatic_Operation = TRUE

What went wrong:
The sensor has failed but normal automatic operation continues.

How do we know:
A failed sensor must prevent normal automatic operation.


## Violation 8 — C8

Constraint:
Barrier_Failure → Safety_Monitor_Alert

Violation:
Barrier_Failure = TRUE
Safety_Monitor_Alert = FALSE

What went wrong:
The barrier has failed but the safety monitor gives no alert.

How do we know:
A barrier failure must generate a safety-monitor alert.
