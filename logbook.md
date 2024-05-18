# Logbook (inverse chronological order)

## One Joint

I'm currently focused on getting one joint completely built, controllable, and characterized.

#### Development Checklist for single interphalangeal joint
##### 1. Mechanical Design
- [x] Implement basic gearbox.
- [x] Test out basic gearbox.
- [x] Implement custom rotated transmission for compactness.
- [ ] Test out custom rotated transmission.
- [ ] Implement clean design for finger housing (and easy assembly).
- [ ] Compose the interphalangeal joints to make 2 joints in series.
##### 2. Control System Design
- [x] Derive MPC controller for impedance control via current sensing.
- [x] Formalize MPC controller design in a small whitepaper.
- [ ] Calibrate MPC controller gains.
- [ ] Test out MPC controller on simple servo.
- [ ] Test out MPC controller on custom interphalangeal joint.
##### 3. Hardware Design
- [ ] Implement basic end-to-end circuit (shunt resistor for current, encoder, microcontroller).
- [ ] Decide if I want to centralize all of the electronics and control or if they should be partially distributed via CAN bus for easier wiring.
- [ ] Design PCBs.
- [ ] Get PCBs made.

### May 18th, 2024
I designed the MPC controller for impedance control (stiffness/damping) using current sensing! I even wrote up a whitepaper that walks through the derivation and has a psuedocode section for algorithm implementation.

I also worked a bit on the rotated transmission and figured out a way to make everything much more compact.



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
