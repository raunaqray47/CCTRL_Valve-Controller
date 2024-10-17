# CCTRL Valve Controller Project using SPPA-T3000 and SIMATIC-S7 Controller

This project implements a Continuous Control (CCTRL) Valve using Siemens' SPPA-T3000 distributed control system. The CCTRL Valve is designed to operate in both manual and automatic modes, with features for setpoint adjustment, error calculation, and PID control.

Components
The CCTRL Valve implementation consists of the following main components:

    CCTRL Block: The core control block for the valve
    SPADJ (Set-Point Adjuster): Controls and sets the valve's setpoint
    SUB (Subtractor): Compares setpoint with actual output to determine error
    MONIT Block: Sets alarms and levels for abnormal conditions
    Level Indicators: Provide graphical display of valve position in the Plant View

Functionality

Manual Mode

    Allows direct opening and closing of the valve as required by the operator

Automatic Mode

    Valve opens and closes based on predefined conditions
    Setpoint determines the maximum opening level of the valve

Control Logic

    SPADJ block sets the desired setpoint
    SUB block calculates the error by comparing setpoint with actual output
    Error is fed into the CCTRL block
    PID conditions are configured within the CCTRL block
    MONIT block monitors for abnormal conditions and triggers alarms
    Output is mapped to level indicators for visual representation

User Interface

    Configuration Mode Design: For setting up the control logic
    Operation Mode: For real-time monitoring and control
    Faceplates: Provide detailed control and status information
    Plant Display: Offers a graphical overview of the valve system

Configuration Mode Design - 
        
        ![Configuration Mode](https://github.com/user-attachments/assets/bcf89093-1b16-40c2-9a67-673cad26f71e)

Operation Mode Design - 
        
        ![Operation Mode](https://github.com/user-attachments/assets/36797347-ff65-4abc-9c8c-f47761726a41)

Faceplate when Valve is closed
        
        ![Faceplate](https://github.com/user-attachments/assets/18dbae07-058d-4091-b4d2-88bb91874284)

Faceplate when Valve is Open
        
        ![Faceplate_Working](https://github.com/user-attachments/assets/830958a7-48e9-4d1a-915d-9d02aa109771)

Implementation Details

    Platform: SPPA-T3000 Distributed Control System
    Communication Protocol: PROFIBUS DP for field-level communication

Plant Display - 
        
        ![Plant Display](https://github.com/user-attachments/assets/45f4b004-ec37-4f96-b5e8-63433e81d6fc)



