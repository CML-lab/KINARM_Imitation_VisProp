# KINARM_Imitation_VisProp
Imitation with cuing by vision or proprioception, for the Kinarm Exo

This code implements an Imitation Task on the Kinarm Exo (BKIN Technologies).

The task allows for two flavors of imitation: copying of a visually cued cursor trajectory, or copying of a proprioceptively cued motion trajectory (i.e., passive movement of the arm). The cued trajectory consists of one to three chained segments, where each segment can be specified as linear, quadratic, or cubic Bezier curve. Auditory cues are present to indicate the start/end of the demonstrated action, and a go signal to cue the individual to move. Trial end is determined as a long pause in the movement.

This code includes the Simulink solution file, the built Simulink model file, and trial tables to implement a basic experiment. It has been compiled for Dexterit-E 3.7.

***Note, this code uses the PID (position) controller in Dexterit-E. Extreme care must be taken when specifying motion trajectories to ensure no discontinuities or abrupt changes in speed and/or direction, as this will create an extremely unpleasant experience for the participant.***

*Also note, this code has only been written and compiled for the Kinarm Exo system. Modifications to the Simulink code are required to implement this on other Kinarm systems.*
