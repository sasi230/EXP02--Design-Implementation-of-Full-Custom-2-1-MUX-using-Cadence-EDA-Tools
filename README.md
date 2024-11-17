# EXP02--Design-Implementation-of-Full-Custom-2-1-MUX-using-Cadence-EDA-Tools

## Aim:
To design and implement a 2:1 multiplexer (MUX) circuit using Cadence EDA tools, analyse its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

## Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

## Circuit Diagram:
![WhatsApp Image 2024-11-15 at 3 07 27 PM (1)](https://github.com/user-attachments/assets/644f306e-2325-44c7-a998-ed93c725ae46)


## PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence
1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


#### i)	Procedure for Creating New Library.
•	File –New – Library
•	Name : Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK
#### ii)	Create Schematic Cell view.
+	Go to 1st window i.e virtuoso(CIW)
+	File-New-Cell view
+	Setup the new file form
	  Library: Select the one you a created.
	  Cell : Give the experiment name Ex: Inverter View_Schematic
	  Type: Schematic press OK
+	Add the required components from the libraries and make the connections.
+	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
+	Click on browse. This opens the library browser
+	Now select the appropriate library for components like
+		Gpdk45 ------------------------nmos1v,  pmos1v
+	Create Input and Output pins
+	Make the connections by using fixed narrow wire key
+	Click Check and Save button

![Screenshot 2024-09-28 112915](https://github.com/user-attachments/assets/f7e20726-2a2f-4ded-ae82-913d4ce806e5)


 
#### iii)	Creating the Symbol for schematic Cell view
+	In the schematic window, execute 	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
+	Now Symbol generation form appears. Click Ok If No changes required
+	A new window with with default symbol is created.
+	Edit the symbol if you want to give actual symbol shape else continue.
+	Execute Create-Cell view-from cell view
+	Library Name and Cell Name must be same which you have used for schematic. Press OK
+	Check for the position of pin side.Prss OK
+	Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot 2024-09-28 112922](https://github.com/user-attachments/assets/4b90a405-c2bf-4bf6-97e7-1daae06bce8c)



#### iv)	Creating the new test cell view
+	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
+	Follow the step 3(ii) d to make the required connections
![Screenshot 2024-09-28 115112](https://github.com/user-attachments/assets/923e2265-fa73-431b-95e1-437cfccb277c)


#### Analog simulation by SPECTRE.
+	In test cell view window
+	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
+	Execute Simulation -- Net list and Run


## For Transient Analysis Settings and Output
 ![image](https://github.com/user-attachments/assets/080dc6ef-4a28-4e49-8a0e-bf1085bb5313)

![Screenshot 2024-11-10 144855](https://github.com/user-attachments/assets/a0cd34fb-7c14-4100-b899-1b6333f9ec7f)



 



 

## Results:
1.	The experiment successfully demonstrated the design and implementation of a 2:1 MUX using Cadence EDA tools. 
2.	The successful verification through schematic, layout, and simulation underscores the effectiveness of using Cadence EDA tools for digital circuit design.
