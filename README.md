# open-manus
An open-source 3D-printed direct-drive bionic hand. Manus is latin for hand.
### Motivations
I've previously made an open-source differential drive platform, quadruped, and star tracker, which all had interesting design, control, and mechanical challenges. My day job is currently a Machine Learning Research Engineer at a legal AI startup called [Harvey](https://www.harvey.ai) where I work on composing large language models into useful legal assistants, but ultimately my passion (and foray into machine learning) has always been robotics. Currently, I'm most interested in machine learning/reinforcement learning in the context of robotics, and I feel that building and training models to control a bionic hand will function to keep me up-to-date with the machine learning literature and keep me connected to my first love (robotics).

There are many odes to [Ismail al-Jazari](https://en.wikipedia.org/wiki/Ismail_al-Jazari) throughout this project (e.g. the RL model being named Jazari). He was a Muslim polymath inventor from the 12th century known as the "father of robotics" due to his groundbreaking work in automata, and happens to be a personal inspiration of mine.
### High-Level Milestones
 - [x] _**[Mechanical]**_ Joint prototype. (See [May 5th update in logbook](logbook.md#older-than-may-5-2024))
 - [ ] _**[Mechanical]**_ Joint prototype with compact inline motor (custom transmission).
 - [ ] _**[Mechanical]**_ Control / Torque analysis.
 - [ ] _**[Mechanical]**_ Full Forefinger prototype.
 - [ ] _**[Control]**_ Finger range-of-motion analysis.

TODO: Fill this out for a longer horizon (control, RL, planning, etc).

TODO: Formalize success criterion.

### Logbook
See [the logbook](logbook.md) for detailed progress updates.

### Helpful Resources
 - [Will Cogley's Bionic Hand](https://www.youtube.com/watch?v=Iej2jkwU-ts) - I found his videos to be deeply interesting, but felt conflicted about the wire-driven joints. I felt that a direct-drive hand would make assembly/control/maintenance easier, and posed some interesting challenges, so decided to make my own direct-drive design. Ultimately, this was a great project, and his videos are wonderful to watch, even if only for entertainment.

### Tools used
 - [3D Printer] Slightly modified Prusa MK3 (reprinted all printer parts using Formlabs Fuse 1 SLS Printer).
 - [Literature Review] Zotero.
