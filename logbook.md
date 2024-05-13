# Logbook (inverse chronological order)

## One Joint

I'm currently focused on getting one joint completely built, controllable, and characterized.

#### Development Checklist for One Finger (One Joint)
##### 1. Initial Control Implementation
- [ ] Basic Control System: Implement basic control algorithms (e.g., PID control) for motor positioning.
- [ ] Integration: Assemble the joint with motors and initial control system.

##### 2. Software-Controlled Compliance
- [ ] Decide on how to measure torque (sensor or current modulation?).
- [ ] Sensor Integration: Add force/torque sensors to the joint.
- [ ] Feedback Loop: Develop control algorithms for compliance (e.g., impedance control).
- [ ] Testing and Calibration: Test the compliance control and calibrate the system for optimal performance.

##### 3. Deep Control Analysis
- [ ] Data Collection: Collect data on joint movement, response time, and accuracy.
- [ ] Performance Metrics: Analyze metrics such as settling time, rise time, overshoot, and steady-state error.
- [ ] Optimization: Optimize control algorithms based on analysis results.

##### 4. Adaptive Control Implementation
- [ ] Algorithm Development: Implement adaptive control algorithms (e.g., MRAC, STR).
- [ ] Simulation: Use simulation tools (e.g., MATLAB/Simulink) to test adaptive control strategies.
- [ ] Real-world Testing: Apply adaptive control to the physical joint and iterate based on performance.

##### 5. Torque Analysis
- [ ] Calculation: Calculate the required torque for various tasks.
- [ ] Sensor Feedback: Use torque sensors to measure actual torque output and loads.
- [ ] Control Adjustments: Adjust control algorithms to ensure accurate torque modulation.

##### 6. Estimating Full Hand Scale
- [ ] Joint Measurement: Measure the physical dimensions and performance of the developed joint.
- [ ] Scaling Calculation: Use the joint dimensions to estimate the size of the full hand.
- [ ] 3D Modeling: Create a 3D model of the full hand based on the estimated dimensions.

##### 7. Rendering and Visualization
- [ ] Export Models: Export CAD models to 3D rendering software (e.g., Blender, KeyShot).
- [ ] Generate Renders: Create visual renders and animations of the joint and full hand models.

##### 8. Documentation and Iteration
- [ ] Thorough Documentation: Document design choices, control algorithms, and performance data.
- [ ] Iterative Improvement: Continuously test, refine, and improve each component based on feedback and performance.

##### 9. Make first video

### May 5, 2024
Updated the repo readme, added milestones, assets, logbook, and motivations.
Also, drafted a schematic for the transmission that will allow me to rotate the motor 90 degrees to be inline with the rest of the joint without jutting out:

<img src="assets/transmission.png" width="425"/>

### Older than May 5, 2024
I am just summarizing these, since I didn't write logs for some of the sparse earlier work I did here.

First, I created a bare-bones test to recreate the servo gearbox from scratch. The goal here was to prove that I can replicate the gearbox in a parameterized manner, such that I can integrate it into the body of the finger for compactness.

<img src="assets/mk0.png" width="425"/>

Then, I built a simple enclosure around it, since the gearbox was snagging due to plate flexture.


<img src="assets/mk1.png" width="425"/> <img src="assets/mk1_section_view.png" width="425"/> 

Then, I experimented a bit with magnetic encoder placement.


<img src="assets/mk2.png" width="425"/> <img src="assets/mk2_section_view.png" width="425"/> 

Then, I added an end-effector to get a better feel for the motor torque.


<img src="assets/mk5.png" width="425"/> <img src="assets/mk5_section_view.png" width="425"/> 

Then, I did some more work around the encoder to better conform to the narrow specifications for the distance between the magnet and the encoder itself. I also connected the encoder to the end-effector to be able to couple their movements for easier testing.


<img src="assets/mk6.png" width="425"/> <img src="assets/mk6_section_view.png" width="425"/> 
