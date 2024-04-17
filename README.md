# 4BIT_RIPPLECOUNTER
# AIM: 
To simulate and synthesis  4bit ripple counter using vivado. 
# APPARATUS REQUIRED: 
vivado 2023.2 software. 
# PROCEDURE: 
STEP:1 Start the vivado software, Select and Name the New project. 
STEP:2 Select the device family, device, package and speed. 
STEP:3 Select new source in the New Project and select Verilog Module as the 
Source type. 
STEP:4 Type the File Name and module name and Click Next and then finish 
button. Type the code and save it. 
STEP:5 Select the run simulation and then run Behavioral Simulation in the 
Source Window and click the check syntax. 
STEP:6 Click the simulation to simulate the program and give the inputs and 
verify the outputs as per the truth table. 
STEP:7 compare the output with truth table.
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/4BIT_RIPPLECOUNTER/assets/154305926/324dfe68-4985-401a-9f0c-7df90b08265e)
# T- Flip Flop
![image](https://github.com/RESMIRNAIR/4BIT_RIPPLECOUNTER/assets/154305926/2c234c0e-2c48-4688-920b-a43ea6582112)
# D - Flip flop
![image](https://github.com/RESMIRNAIR/4BIT_RIPPLECOUNTER/assets/154305926/7fb0da71-700b-4a53-b2c1-2afa523e89c4)
# verilog code
module synchronous_up_counter(

input wire clk,   // Clock input

input wire reset, // Reset input

output reg [3:0] count // 4-bit output
);

// Reset the counter to 0 when reset is active

always @(posedge clk or posedge reset)

begin

if (reset)

    count <= 4'b0000;
    
else

    count <= count + 1; // Increment the count on each clock cycle
end

endmodule
# output
![WhatsApp Image 2024-04-17 at 13 20 19_8af7fa36](https://github.com/lathika024/4BIT_RIPPLECOUNTER/assets/165888553/a505a4de-1cbe-44a6-b2f4-f4cc37d327c4)
# result 
Thus the 4bit ripplecounter is verified successfully 

