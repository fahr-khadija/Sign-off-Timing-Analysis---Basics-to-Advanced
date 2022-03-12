![STA_Banner](https://user-images.githubusercontent.com/100168693/158027369-eb20fa1b-73dd-47c9-a26b-933dc1e13eb1.jpg)



# Overview

The workshop covers all the basic concepts in STA and Timing constraints. It starts with basics of Static Timing Analysis, timing paths, startpoint, endpoint and combinational logic definitions. It explains setup and hold checks, how STA tools calculate setup and hold violations. Then it slowly builds up to cover all aspects of STA like multiple types of timing paths, design rule checks, checks on async pins and clock gates. After that we go into slightly advanced topics like Time borrowing on latches, timing arcs, cell delays and models, impact of clock network on STA. Since STA and timing constraints go hand in hand the workshop covers basics of all the timing constraints that an engineer should know for STA like clock definitions, clock groups, clock characteristics, port delays and timing exceptions. Each day of the workshop is associated with labs so attendees can apply the concepts they have leant that day on practical examples and deepen their knowledge of the concepts


# Sign-off-Timing-Analysis---Basics-to-Advanced

- [Sign-off Timing Analysis - Basics to Advanced](#sign-off-timing-analysis---basics-to-advanced) 
 

* - [Day 1](#day-1) 
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
  * - [Day 2](#day-2)
    + [- Other timing checks](#--other-timing-checks)
    + [- Design Rule Checks](#--design-rule-checks)
    + [- Latch Timing](#--latch-timing)
    + [- STA Text Report](#--sta-text-report)
    + [- Day 2 labs -](#--day-2-labs--)
      - [Liberty Files,](#liberty-files-)
      - [SPEF,](#spef-)
      - [timing reports](#timing-reports)
     
  - [Day 3](#day-3)
    + [- Multiple Clocks](#--multiple-clocks)
    + [- Timing arcs and Timing Sense](#--timing-arcs-and-timing-sense)
    + [- Cell Delays and Clock Network](#--cell-delays-and-clock-network)
    + [- Setup and Hold Detailed](#--setup-and-hold-detailed)
    + [- STA Text Report](#--sta-text-report)
    + [- Day 3 labs](#--day-3-labs)
      - [Understanding full reg to reg STA analysis,](#understanding-full-reg-to-reg-sta-analysis-)
      - [slack computation and review setup check report](#slack-computation-and-review-setup-check-report)
     
 - [Day 4](#day-4)
    + [- Lectures and Labs](#--lectures-and-labs)
    + [- Crosstalk and Noise](#--crosstalk-and-noise)
    + [- Operating modes and other variations](#--operating-modes-and-other-variations)
    + [- Clock Gating Checks](#--clock-gating-checks)
    + [- Checks on Async Pins](#--checks-on-async-pins)
    + [- Day4 labs](#--day4-labs)
      - [Understanding clock gating check,](#understanding-clock-gating-check-)
      - [async pin checks](#async-pin-checks)
      
      
 - [Day 5](#day-5)
    + [- Clock groups](#--clock-groups)
    + [- Clock properties](#--clock-properties)
    + [- Timing exceptions](#--timing-exceptions)
    + [- Multiple modes](#--multiple-modes)
    + [- Day 5 labs](#--day-5-labs)
      - [Revisit slack computation,](#revisit-slack-computation-)
      - [understand CRPR and ECO insertion](#understand-crpr-and-eco-insertion)

 

 

## Day 1

####  - STA Definition
Static timing analysis (STA) is a method of validating the timing performance of a design by checking all possible paths for timing violations. STA breaks a design down into timing paths, calculates the signal propagation delay along each path, and checks for violations of timing constraints inside the design and at the input/output interface.


####  - Timing Paths
####  - Timing path elements
####  - Setup & Hold Checks
####  - Slack Calculation
####  - SDC Overview
####  - Clocks
####  - Generated Clocks
####  - Boundary Constraints
####  - Day1 Labs - 
   ##### OpenTimer Introduction,
   ##### Inputs to OpenTimer, 
   [run.log](https://github.com/fahr-khadija/Sign-off-Timing-Analysis---Basics-to-Advanced/files/8238024/run.log)

   
   ##### Constraints creation 
   /home/khadija.fahr/Desktop/openSTA_sta_workshop/vlsideepdive_openSTA_labs/lab1/simple.sdc
   ## reading liberty model
**read_liberty ../sky130_fd_sc_hd__tt_025C_1v80.lib
## reading netlist model
read_verilog simple.v
link_design simple
## Parsing constraints
read_sdc -echo simple.sdc
## report timing reports for 5 paths
report_checks -group_count 5 **

   
   ##### OpenTimer RunscriptPaste 

/home/khadija.fahr/Desktop/openSTA_sta_workshop/vlsideepdive_openSTA_labs/lab1/run.tcl

  
## Day 2
####   - Other timing checks

####   - Design Rule Checks


####   - Latch Timing

####   - STA Text Report

####   - Day 2 labs -  

   ##### Liberty Files,
   
   ##### SPEF, 
   
   ##### timing reports 
   
   
  ## Day 3
####   - Multiple Clocks  
####   - Timing arcs and Timing Sense
####   - Cell Delays and Clock Network
####   - Setup and Hold Detailed
####   - STA Text Report
####   - Day 3 labs 
   #####  Understanding full reg to reg STA analysis,
   #####  slack computation
   #####  review setup check report
   
    
## Day 4
####    - Lectures and Labs 
####    - Crosstalk and Noise
####    - Operating modes and other variations
####    - Clock Gating Checks
####    - Checks on Async Pins
####    - Day4 labs 
   #####  Understanding clock gating check,
   #####  async pin checks 
   

## Day 5
####    - Clock groups
####    - Clock properties
####    - Timing exceptions
####    - Multiple modes
####    - Day 5 labs 
   #####  Revisit slack computation,
   #####  understand CRPR and ECO insertion
   
   
   


 
   
   
    
   
   





