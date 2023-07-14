
# TCL Workshop: From Introduction to Advanced Scripting Techniques in Design and Synthesis

TCL scripting plays a crucial role in the field of VLSI design and verification, making it an indispensable tool for semiconductor engineers. VLSI projects involve complex tasks such as chip design, simulation, verification, and manufacturing, and TCL scripting provides an efficient and flexible way to automate these processes. With TCL, engineers can write scripts to automate design tasks, perform simulations, analyze data, and generate reports, significantly reducing the time and effort required for repetitive tasks. TCL also offers excellent integration capabilities, allowing seamless interaction with other EDA tools and languages. Moreover, TCL scripting provides a high level of control and customization, enabling engineers to create complex workflows and implement design methodologies specific to their requirements. Overall, TCL scripting empowers VLSI engineers to enhance productivity, streamline workflows, and accelerate the development and verification of advanced integrated circuits.

- [Workshop Details & Agenda](#Workshop-Details-&-Agenda)
- [Day-wise Workshop Progress](#Day-wise-Workshop-Progress)
- [Quality of Results (QoR)](#Quality-of-Results-(QoR))
- [Conclusion](#Conclusion)
- [Acknowledgements](#Acknowledgements)

# Workshop Details & Agenda

VLSI System Design Corp. Pvt. Ltd. had proposed this 5 days workshop entitled as "TCL Workshop: From Introduction to Advanced Scripting Techniques in Design and Synthesis
" from 5th July 2023 to 9the July 2023 with the guidance of Mr. Kunal Ghosh, Co-Founder, VSD Corp. Pvt. Ltd. and Ms. Geetima Kachari who had been working as the Teaching Assistant throughout the entire workshop. The agenda for the workshop is as follows :

Day 1 (5th July 2023) : Serving as the foundation, introduction to the core concepts and tasks of TCL. 

Days 2 & 3 (6th & 7th July 2023): Immersing in the art of variable creation and processing constraints. 

Day 4 (8th July 2023) : Introduction to Yosys synthesis tool, understanding memory module RTL descriptions, and mastering gate level netlist descriptions.

Day 5 (9th July 2023) : Quality of Results (QOR) generation, optimization to precise WNS and FEP ana# Day-wise Workshop Progress

- [Day 1 5th July 2023](#Day-1-5th-July-2023)
- [Day 2 6th July 2023](#Day-2-6th-July-2023)
- [Day 3 7th July 2023](#Day-3-7th-July-2023)
- [Day 4 8th July 2023](#Day-4-8th-July-2023)
- [Day 5 9th July 2023](#Day-5-9th-July-2023)



# Day 1 5th July 2023
# Tasks of the Day :

     • Invoke TCL Command by accepting command line arguments
    • Deal with issues to pass command line argument to TCL Script (Eg. No Argument, Multiple Arguments, Argument doesn't exist)
# Results : 

Case 1) Normal Command Line Argument Passing

![DAY_image1](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/1719184d-02ab-46e9-bbb7-4c38e9aa19fe)

Case 2) Command Line Argument Doesn't Exist

![cannot_find_csv](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/96da025d-e112-49e5-a0c7-00eedf07b5e6)

# Day 2 6th July 2023
# Tasks of the Day :

    • Auto Variable Creation
    • Checking if provided directories exist at respective locations, display an error if not found.....
    • Convert the inputs into a format that can be passed to Yosys Synthesis Tool

# Results 
1) Passing Inputs Path from .csv file to the Scripts :

![Screenshot from 2023-07-11 16-40-44](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/09b8aa02-2966-4726-8fd5-a61186e3192d)

3) Checking the directories for given input path exists at respective locations or not :

![check_the_presenceofpathsandnames](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/8a57efea-997a-466c-9eac-38063c6ded99)

3) Display an Error if the directory is not found at given location :

![Return_errorif parametersarenotpresent](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/78385e52-fd93-456a-8d6c-44e33f755332)


# Day 3 7th July 2023

# Tasks of the Day :

    • Read the Clock, Input & Output Constraints from the file and create Synopsys Design Constraints (SDC) Format .sdc file
    • Take care of the bus port to create SDC file
    • Verify the generated .sdc file

# Results 

1) Reading the sdc 

![Read_constraintfileincsvandconverttosdc](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/2605397e-07fd-4be1-ae24-a0e3ea4467b5)

2) Generated SDC File and observing the input ports

   ![sdc_wrt_input_ports](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/4e25258e-0153-4fa8-962a-012c58af3516)


# Day 4 8th July 2023

# Tasks of the Day :

    • Create a synthesis script that can be passed as an argument to Yosys Synthesis Tool
    • Run the hierarchy check to verify if all RTL modules are correctly present or not, raise an error if not.
    • Observe the generated netlist and remove the redundant part from it

# Results

1) Hierarchy Check PASS

![Hierarchy_check_pass](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/44ab5740-0682-424b-9252-f436385472b6)


2) An Example where Hierarchy Check gets FAIL

![DAY4_hierfail](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/c654ce5d-7d9b-4758-823b-7742525ae846)


3) Log file while generating SDC

![DAY4Logfile_message_reg_error (1)](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/42696cdd-fb95-4b96-804d-eb26d9a1f160)

4) Genarating script for yosys tool

![Day5_synthesized_netlist](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/b57fa042-10c0-47f1-b14e-17e8400c2624)

5) Snapshot of Netlist generated by Yosys Tool

![Day4netlist](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/70243752-4159-4ae6-bcbc-c7a9cc8495ad)

# Day 5 9th July 2023

# Tasks of the Day :

    • Create a constraint .timing file from the .sdc file which can be applied to OpenTimer tool
    • Take care of all bits of the bus while creating the .timing file 
    • Create a .conf file input script for the OpenTimer tool
    • Quality of Results (QoR) Generation


# Results

1) .conf File Input Script for OpenTimer tool

![Day5_conf_file](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/8a56cc78-0c2c-44c6-bcc8-6334f5fb50e8)


2) Snapshot of generated .timing file
   
![Day5_timing_file](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/5d2f8977-287a-40ce-919b-a0701873fc8d)


# Quality of Results (QoR)


![QOR_final](https://github.com/Nripench/VSD_5_DAYS_TCL_WORKSHOP/assets/138991348/49a94e88-218d-477f-9d7c-4835a65bf173)


# Conclusion 

An Automation has been successfully created using TCL scripting which will take the input from the user as RTL Verilog Code files and library paths, process the pre-layout synthesis and run the static timing analysis (STA) and displays the Quality of Results (QoR).

# Acknowledgments

1) Mr. Kunal Ghosh, Co-Founder, VSD Corp. Pvt. Ltd.

2) T R Visruat

3) Geetima Kachari









  
