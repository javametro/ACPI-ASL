## ACPI States
* ACPI is defining states for the whole system and for each component independently

### System states
* G0(S0) : system fully ON
* G1 : sleeping. Several sub-levels are defined here
* S1 : power on suspend
* S2 : suspend to RAM
* S3 : standby 
* S4 : hibernate
* G2(S5) : Soft OFF, System still listening to some events (keyboard, USB, network) in order to start if received.
* G3(S6) : Mechanical OFF. Only CMOS is running

### Device states
* D0 : ON
* D1, D2 : intermediate, depend on device. May not be present
* D3 : OFF