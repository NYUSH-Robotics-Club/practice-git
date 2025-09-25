PID motor control is used to control motor's movement through feedback control loop. It compares what motor is doing vs what we want it to actually do -> calculate the correction. 

The goal is to reach a target (aka setpoint) while avoiding overshooting/oscillating.

PID stands for

    P - Proportional 
        Corrective force is proportional to size of error. If very far from target apply very strong corrective force. Apply gradually smaller force as it approaches target.

    I - Integral
        Accumulation of past errors or the area under the error curve over time. I term will gradually increase output to overcome small errors that persist. Has chance of overshooting if influence is too strong.

    D - Derivative
        Responds to the rate of change of error. The D term counteracts fast changes in error. Reduce overshoot and oscillation by slowing the system down as it approaches the target.