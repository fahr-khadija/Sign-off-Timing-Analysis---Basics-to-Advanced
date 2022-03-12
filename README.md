![STA_Banner](https://user-images.githubusercontent.com/100168693/158027369-eb20fa1b-73dd-47c9-a26b-933dc1e13eb1.jpg)


# Sign-off-Timing-Analysis---Basics-to-Advanced

- [Sign-off Timing Analysis - Basics to Advanced](#sign-off-timing-analysis---basics-to-advanced) 
  * [Day 1](#day-1) 
      - [- STA Definition](#--sta-definition) 
      - [- Timing Paths](#--timing-paths) 
      - [- Timing path elements](#--timing-path-elements) 
      - [- Setup & Hold Checks](#--setup---hold-checks) 
      - [- Slack Calculation](#--slack-calculation) 
      - [- SDC Overview](#--sdc-overview) 
      - [- Clocks](#--clocks) 
      - [- Generated Clocks](#--generated-clocks) 
      - [- Boundary Constraints](#--boundary-constraints) 
      - [- Day1 Labs -](#--day1-labs--) 
        * [OpenTimer Introduction,](#opentimer-introduction-) 
        * [Inputs to OpenTimer,](#inputs-to-opentimer-) 
        * [Constraints creation](#constraints-creation) 
        * [OpenTimer RunscriptPaste](#opentimer-runscriptpaste) 
 


Static timing analysis (STA) is a method of validating the timing performance of a design by checking all possible paths for timing violations. STA breaks a design down into timing paths, calculates the signal propagation delay along each path, and checks for violations of timing constraints inside the design and at the input/output interface.

The workshop covers all the basic concepts in STA and Timing constraints. It starts with basics of Static Timing Analysis, timing paths, startpoint, endpoint and combinational logic definitions. It explains setup and hold checks, how STA tools calculate setup and hold violations. Then it slowly builds up to cover all aspects of STA like multiple types of timing paths, design rule checks, checks on async pins and clock gates. After that we go into slightly advanced topics like Time borrowing on latches, timing arcs, cell delays and models, impact of clock network on STA. Since STA and timing constraints go hand in hand the workshop covers basics of all the timing constraints that an engineer should know for STA like clock definitions, clock groups, clock characteristics, port delays and timing exceptions. Each day of the workshop is associated with labs so attendees can apply the concepts they have leant that day on practical examples and deepen their knowledge of the concepts
