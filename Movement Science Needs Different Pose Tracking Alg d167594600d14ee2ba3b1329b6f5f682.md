# Movement Science Needs Different Pose Tracking Algorithms

### Research Paper Interpretation and Notes

by Adit Magotra 

The original paper can be found [here](https://arxiv.org/pdf/1907.10226.pdf)

## 1. Abstract



- The problem statement basically states that  **Pose Tracking Algorithms** poorly estimate the movement science
- They use: noisy data (manually labeled)
- They ignore: Important physical factors like Velocity, Acceleration, 3D Coordinates, and Force

<aside>
👨🏻‍💻 Keywords: Movement Science | Computer Vision | Pose Estimation

</aside>

## 2. Movement Data



We don’t just need data. We need **Meaningful Data**.

Eg. Quantified Data as a biomarker for diseases 

Studying movement is very important as well

<aside>
ℹ️ **Quantified Data**: Measurement of aspects of our like (Like Blood Oxygen Tracking)

</aside>

Some contributions to movement science - 

### Neuroscience

- Understanding the neural basis is the key to understanding movement because movement is the way an animal interacts with its environment
- Done by studying the outputs (velocity, force) and matching them with the neural signals
- Helps in finding Neural correlation with activities for further research
- 

---

### Biomedical Engineering

- Movement data subject to engineering tools
- Analyze and simulate the movement statistics
- Helps in finding out parameters for diseased limbs and organs used in locomotion activities

---

### Sports and Exercise Science

- Used to improve the quality of the game of sportspeople
- Done by analyzing metrics like Position, Velocity, etc. of the player
- Correlated with performance and used to give feedback
- May even predict eventual success in sports

---

### Psychology

- Relation between mental activity and observable factors (like movement)
- Used to study responses to a particular action and test theories
- Cognition and Perception theories have been previously tested and found to be accurate

---

### Physiology

- Human body movement data to get movement mechanisms
- Factors can be muscle activation / metabolic energy
- Example - At the intramuscular scale, one study found that motor units within a given muscle
are activated over a small spatial range during human standing
- Helps in making mechanistic models of movement

---

### Rehabilitation

- Goal - To use movement data as a diagnostic tool to quantify the progress post-treatment for diseases like Parkinson’s Disease and Movement Disorders.
- Example - Variability in gait motion is directly linked to fall-avoidance models
- Can be used to better the quality of medical rehabilitation using movement as data

<aside>
ℹ️ Gait Motion - Sequence of limb movements to achieve locomotion

</aside>

---

### Biophysics

- Ti find out more info about how humans walk and if it’s the most efficient manner possible
- Used by analyzing movement, metabolic and feedback data
- Predicts the relationship between these and other factors like stability

---

### Robotics

- Human and Animal movement data serves as inspiration for robot movement
- Need to replicate movement techniques in a low cost and quantifiable environment

---

### Other Disciplines

- Used in several other fields
- Example - Used as a metric to find body language emotion in social science || Analyzing human behavior to filter suspicious activity from security cameras

## 3. Pose tracking promises to transform the scale of movement science



- The moving industry is huge
- However, traditional tools limit the scope
- CV based human pose estimation may transform movement Science (Can catch complex movements occurring in natural environments)
- The majority of research is done in labs that limit the scope of movement variation capture
- Some other limiting factors are the high cost of sensors, lack of variation in data, small sample data sizes

## 4. Pose tracking algorithms need to estimate different movement quantities



![Untitled](Movement%20Science%20Needs%20Different%20Pose%20Tracking%20Alg%20d167594600d14ee2ba3b1329b6f5f682/Untitled.png)

- Movement Science needs a good estimate of physical quantities and dimensions
- The major focus of pose-tracking algorithms has been on 2D data while actual impacts are only shown in 3D data
- Consecutive time frames are treated as statistically independent and the underlying dynamical structure of the pose statistics is ignored. Results in misestimates
- Current data does not capture actual types of movements in movement science
- Result in an increased mean error and inaccurate estimations of movement

### Three-dimensional position, velocity, and acceleration

- More and more pose tracking algorithms are aiming for 3D estimates
- However, Tracking of time, velocity, and acceleration is minimal
- It May be possible by changing the Algorithms and ground truth benchmarks
- Possible to incorporate into the algorithm camera motion to obtain 3D depth
information
- Minimization of errors in velocity and acceleration, not just pose, can be added to the objective functions of the algorithms

### External Contact Forces

- Quantifying forces is important in many applications
- Cannot be directly estimated from mass and acceleration because such a system is ‘statically indeterminate’
- Impossible to measure force through pose estimation algorithms and video frames

### Absolute mass, length, and inertia

- Important to understand how movements differ by body types
- Needed to estimate internal forces
- Can predict relative measures through segmentation and ratios but absolute measures are crucial for movement science
- One way to rectify this is by using computer vision to estimate the true size and scale of a known object in the
background and use this information to estimate the size of the person or animal in the image
- Other factors like air resistance can also be used to make meaningful inferences

### Pose tracking with task and subject generality

- Movement differs by task and demographics
- Unclear about racial/demographic bias in AI algorithms due to unbalanced data
- Pose Tracking Algorithms can be improved by taking a diverse range of data from different demographic locations and categories

### Fixed frame of reference

- Estimates of body motion need to be in a fixed frame of reference
- One way to deal with this is to take multiple camera angles
- Could be fixed to a specific object for its frame of reference

## Conclusions



- Progress over the last decade
- Hasn’t affected movement science research majorly as the algorithms do not prioritize quantified data
- Need to design Pose Tracking Algorithms that actually define Movement Science Factors
