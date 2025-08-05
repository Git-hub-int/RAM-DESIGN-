1️⃣# RAM-DESIGN-

COMPANY:- CODTECH IT SOLUTIONS 

NAME:- GARIMA VERMA

INTERN ID:- CT04DH2092

DOMAIN:- VLSI

DURATION:- 4 WEEKS 

MENTOR:- NEELA SANTOSH 

RAM (Random Access Memory) is a type of volatile memory used in digital systems to store and retrieve data quickly. It allows random access, meaning data can be read from or written to any memory location in constant time, regardless of its physical location.

 ▶️In this task implements a Random Access Memory (RAM) module in Verilog HDL with:
 
➡️Independent read and write ports

➡️Configurable data width and address width

➡️Fully synthesizable memory using register arrays

➡️Designed for simulation in Icarus Verilog and waveform viewing with GTKWave

2️⃣Module Interface

Signal	               Direction           	 Description
clk_write	               Input              	Write clock
address_write	           Input            	Address to write to
data_write	             Input	            Data input for writing
write_enable	           Input	       Enables writing on write clock
clk_read	               Input              	Read clock
address_read	           Input	            Address to read from
data_read	Output	       Output             data from memory

3️⃣Testbench Overview 

➡️Simulates writing value 0xC5 to address 0x1B

➡️Reads the memory content before and after writing

▶️Uses two custom tasks:

➡️toggle_clk_write – toggles write clock

➡️toggle_clk_read – toggles read clock

Dumps simulation data to dump.vcd for GTKWave

4️⃣How to Run the Simulation

iverilog -o ram_test ram.v

vvp ram_test

gtkwave dump.vcd

OUTPUT:-
![Image](https://github.com/user-attachments/assets/be13ac8e-653a-4126-9ff2-4ad7a79c4d0f)
