# PLC-FAULT-TOLERANT-CONTROL-ARCHITECTURE
PLC-Based Fault Detection & State Machine Control Framework
Overview :- 
This project implements a layered fault-tolerant industrial control architecture using CODESYS PLC programming.
The system is designed to detect and handle:
Sensor faults
Actuator faults
Process deviation faults
Logic faults
Architecture :- 
The control system is structured into three layers:
Monitoring Layer
Detects sensor, actuator, and process faults using deviation and timeout logic.
Severity Classification
Classifies faults as Minor, Major, or Critical based on deviation thresholds.
Response & State Machine Layer
Implements enum-based state control:
IDLE
RUNNING
RETRY
STOPPED
LOCKOUT
Minor faults trigger controlled retry attempts.
Major faults escalate to system lockout requiring manual reset.
Features :- 
Enum-based deterministic state machine
Fault prioritization logic
Retry mechanism with limit control
Lockout safety handling
Structured Text (ST) implementation
Fully simulated and tested in CODESYS environment
Tools Used :- 
CODESYS PLC Development System
Structured Text (IEC 61131-3)
