# open-manus
An **open-source**, **3D-printed**, **direct-drive**, **1:1.5 scale** bionic hand. Manus is latin for hand.

I'm almost done with the joint connecting the middle and distal phalanges (labeled and highlighted in blue below).

<img src="assets/mk6_render.png" height="250"/> <img src="assets/mk6_hand_bone_anatomy_diagram.png" height="250"/>

#### Table of Contents
1. [Current Status & Logbook](#current-status--logbook)
2. [Motivations](#motivations)
3. [High-Level Milestones](#high-level-milestones)
4. [Helpful Resources](#helpful-resources)
5. [Tools Used](#tools-used)

### Current Status & Logbook
I have a joint with an embedded magnetic encoder working. Currently working on a custom transmission to rotate the motor 90 degrees to be inline to keep the finger compact and the joints serially composable.

<img src="assets/mk6.png" width="250"/> <img src="assets/mk6_section_view.png" width="250"/>  

Also, drafted a schematic for the transmission that will allow me to rotate the motor 90 degrees to be inline with the rest of the joint without jutting out (see schematic below). For the coupler between the motor shaft (1.5mm) and the transmission shaft (2mm) in the diagram, I was unable to find an off-the-shelf solution, so am going to 3d print my own coupler. [Found a nice resource on YT on best practices to 3d print holes](https://www.youtube.com/watch?v=Bd7Yyn61XWQ&pp=ygUOM2QgcHJpbnQgaG9sZXM%3D).

<img src="assets/transmission.png" width="425"/>


See [the logbook](logbook.md) for more detailed progress updates.

### Motivations
I've previously made an open-source [differential drive platform](https://www.adhamelarabawy.com/projects/precision_drivetrain/), [quadruped](https://www.adhamelarabawy.com/projects/open_quadruped/), and [star tracker](https://www.adhamelarabawy.com/projects/open_startracker/), which all had interesting design, control, and mechanical challenges. My day job is currently a Machine Learning Research Engineer at a legal AI startup called [Harvey](https://www.harvey.ai) where I work on composing large language models into useful legal assistants, but ultimately my passion (and foray into machine learning) has always been robotics. Currently, I'm most interested in machine learning/reinforcement learning in the context of robotics, and I feel that building and training models to control a bionic hand will function to keep me up-to-date with the machine learning literature and keep me connected to my first love (robotics).

There are many odes to [Ismail al-Jazari](https://en.wikipedia.org/wiki/Ismail_al-Jazari) throughout this project (e.g. the RL model being named Jazari). He was a Muslim polymath inventor from the 12th century known as the "father of robotics" due to his groundbreaking work in automata, and happens to be a personal inspiration of mine.

### High-Level Milestones
 - [x] _**[Mechanical]**_ Joint prototype. (See [May 5th update in logbook](logbook.md#older-than-may-5-2024))
 - [ ] _**[Mechanical]**_ Joint prototype with compact inline motor (custom transmission).
 - [ ] Finalize scale relative to human hand.
 - [ ] _**[Mechanical]**_ Control / Torque analysis.
 - [ ] _**[Mechanical]**_ Full Forefinger prototype.
 - [ ] _**[Control]**_ Finger range-of-motion analysis.

TODO: Fill this out for a longer horizon (control, RL, planning, etc).

TODO: Formalize success criterion.

### Helpful Resources
 - [Will Cogley's Bionic Hand](https://www.youtube.com/watch?v=Iej2jkwU-ts) - I found his videos to be deeply interesting, but felt conflicted about the wire-driven joints. I felt that a direct-drive hand would make assembly/control/maintenance easier, and posed some interesting challenges, so decided to make my own direct-drive design. Ultimately, this was a great project, and his videos are wonderful to watch, even if only for entertainment.
 - [Nice resource on best practices to 3d print holes](https://www.youtube.com/watch?v=Bd7Yyn61XWQ&pp=ygUOM2QgcHJpbnQgaG9sZXM%3D).

### Tools used
 - [3D Printer] Slightly modified Prusa MK3 (reprinted all printer parts using Formlabs Fuse 1 SLS Printer).
 - [Literature Review] Zotero.
