USING KOHONEN SELF-ORGANIZING NETWORKS
PATRICK JOINER
OF THE UNIVERSITY OF FLORIDA IN PARTIAL FULFILLMENT
OF THE REQUIREMENTS FOR THE DEGREE OF
MASTER OF SCIENCE
UNIVERSITY OF FLORIDA
1993
by
Patrick Joiner
ABSTRACT     vi
CHAPTERS
1     INTRODUCTION     1
2     ANIMATION     3
Conventional Animation     3
Computer-Assisted Animation     3
Computer Animation       4
Control of Computer Animation     5
Explicit Control     5
Procedural Control     5
Constraint-based Control     6
3     ANIMATION OF HUMAN LOCOMOTION     8
Kinematic Specification     8
Keyframe Interpolation     9
Finite State Automaton Control     9
Dynamic Specification     10
Hybrid Approaches     11
The Ideal Controller     12
4     NERVE CELLS     13
Structure     13
Cell Body     14
Dendrites     14
Axon     14
The Synapse     15
Nerve Signal Propagation     16
5     HISTORY OF NEURAL NETWORKS     18
Foundations     18
Early Work     19
Downfall     20
Resurgence     20
Current Status     21
6     NEURAL NETWORK MODELS     22
The Perceptron     22
ADALINE/MADALINE     25
The Hopfield Network     28
The Backpropagation Network     32
The Self-Organizing Network     35
7     KOHONEN SELF-ORGANIZING NETWORKS     36
8      NEURAL CONTROL OF LOCOMOTION     44
Analysis of Locomotion     44
Motor Control     45
Locomotion Control in Animals     48
Locomotion Control in Humans     49
9     THE LOCOMOTION CONTROLLER     51
Neural Basis of the Controller     51
The Human Machine     52
The Kohonen Network     53
Locomotion Data     54
Training     56
The Animation Controller     56
10     RESULTS AND CONCLUSIONS     58
Results     58
Conclusions     61
Limitations     61
Possible Extensions     62
APPENDICES
A     DIGITIZED VIDEOTAPE FRAMES USED FOR DATA ACQUISITION     64
B     DATA USED TO TRAIN THE KOHONEN NETWORK     71
REFERENCES     80
BIOGRAPHICAL SKETCH     83
of the University of Florida in Partial Fulfillment of the
Requirements for the Degree of Master of Science
CONTROL OF THE ANIMATION OF HUMAN LOCOMOTION
USING KOHONEN SELF-ORGANIZING NETWORKS
By
PATRICK J. JOINER
December, 1993
Chairman:  Paul A. Fishwick
Major Department:  Computer and Information Sciences
Animation has been a major part of the entertainment industry since motionpictures were invented.  Although a relatively recent development, computer animationhas quickly emerged as a dominant medium for many fields, not limited to entertainment.
An interesting problem in animation is the realization of the motion of humansand animals.  There is an abundance of data resulting from the study of human andanimal locomotion, and from these data have arisen several approaches to the animationof locomotion.  These different approaches have had varying levels of success,where success is defined as the amount of realism present in the resulting animation.
A logical way to build an animation controller is to simulate the mechanisms ofthe brain.  This is not a trivial task, since little is known about the function of the brain.The best way to approximate the function of the brain is to utilize neural network models.
Kohonen neural networks are a type of neural network model which is based onthe way in which the brain organizes stimuli.  Given a set of input data, a Kohonennetwork can organize the data in a way that makes the control of animation easy for the userand computationally simple for the computer as well, producing realistic output in real time.
We present a method for using Kohonen self-organizing networks to controlthe animation of human locomotion.  This methodology makes it possible to controlhuman locomotion with a high-level script language and is easily adaptable to provide awide range of motions which are not limited to locomotion.
