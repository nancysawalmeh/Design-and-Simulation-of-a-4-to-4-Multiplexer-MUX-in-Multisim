Design and Simulation of a 4-to-4 Multiplexer (MUX) in Multisim

Components Used:
1-AND gates (x4) – To control each input and select the correct data based on the control lines.
2-OR gate (x1) – To combine the outputs of the AND gates and produce the final result.
3-NOT gates (x2) – To invert the control lines where necessary.
4-Select Lines (S1, S0) – Two control inputs that determine which data input is passed to the output.
5-Data Inputs (D0, D1, D2, D3) – Four inputs to the multiplexer.
6-Output (Y) – The final output, determined by the selected input.

Operation: 
The 4-to-4 MUX selects one of the four data inputs (D0, D1, D2, D3) based on the select lines (S1, S0). 
The select lines control the flow of data through the AND gates, enabling only one input at a time. 
The output from all the AND gates is then combined using an OR gate to produce a single output (Y).

Truth Table:
Select Lines (S1, S0)	     Output (Y)
   00	                       D0
   01	                       D1
   10	                       D2
   11	                       D3

  Boolean Expression for the Output:Y = (~S1 * ~S0 * D0) + (~S1 * S0 * D1) + (S1 * ~S0 * D2) + (S1 * S0 * D3)

Steps to Build the Circuit :
1-Insert the required gates (AND, OR, NOT) from the Multisim component library.
2-Connect the select lines (S1, S0) to the AND gates, applying the NOT gates where needed to create complements.
3-Connect the data inputs (D0, D1, D2, D3) to the corresponding AND gates.
4-Combine the AND gate outputs using the OR gate to produce the final output.
5-Simulate the circuit, varying the select lines to observe how the MUX routes the correct input to the output.
