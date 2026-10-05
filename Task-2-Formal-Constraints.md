# Task 2 — Formalize Constraints

## C1
Constraint:
The barrier must not open while a train is present.

Formal Expression:
Train_Present → ¬Barrier_Open


## C2
Constraint:
The barrier must close when an approaching train is detected.

Formal Expression:
Train_Approaching → Barrier_Closed


## C3
Constraint:
Warning lights must be activated when a train approaches.

Formal Expression:
Train_Approaching → Warning_Lights_On


## C4
Constraint:
The audible alarm must be activated when a train approaches.

Formal Expression:
Train_Approaching → Audible_Alarm_On


## C5
Constraint:
The barrier must remain closed while the train is passing.

Formal Expression:
Train_Passing → Barrier_Closed


## C6
Constraint:
The barrier must open only after the train has completely cleared the crossing.

Formal Expression:
¬Train_Present → Barrier_Open


## C7
Constraint:
The system must not rely on a failed train-detection sensor.

Formal Expression:
Sensor_Failed → ¬Normal_Automatic_Operation


## C8
Constraint:
A barrier failure must be detected by the safety-monitoring unit.

Formal Expression:
Barrier_Failure → Safety_Monitor_Alert


## C9
Constraint:
Communication loss must not cause the barrier to open unsafely.

Formal Expression:
Communication_Lost → ¬Unsafe_Barrier_Open


## C10
Constraint:
Emergency conditions must place the crossing into a safe state.

Formal Expression:
Emergency → Safe_State
