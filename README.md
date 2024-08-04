<div align="center">
  <h1>MiniMIPS Multi Cycle Datapath</h1>
  <a href="https://sites.google.com/view/rhythmshah/design-and-implementation-of-minimips-multi-cycle-datapath-using-verilog"><b>Visit my website</b></a>
</div>


## **Objective :**

This project aims to use the MiniMIPS architecture in Verilog Hardware Description Language (HDL) to design and develop a multicycle data path. The MIPS (Microprocessor without Interlocked Pipeline Stages) architecture, well-known for its effectiveness and adaptability, is condensed into the MiniMIPS design. The MiniMIPS architecture is a condensed version of basic microprocessor architecture that executes a million instructions per second. For better resource utilization and to execute all instructions in optimized time, a multicycle datapath is used that caters to the cons of singlecycle datapaths by completing multiple instructions in a single clock cycle.

## **Implementation-**

I created multiple submodules for input and output selection, Dual port RAM, shifters, and the Arithmetic Logic Unit (ALU) which consists of adders, subtractors, and logical operators and a main module that acts as a hub to call these submodules using Verilog HDL. As multicycle datapath has multiple states the control state module is designed using verilog hdl that controls the signals to each submodule in datapath as per mealy state machine. This datapath is tested and verified using testbench in verilog hdl which covers a wide range of instructions. 

## **Features-**

1. 32-bit MiniMIPS architecture datapath.
2. Have numerous storage registers at each stage.
3. The instruction set covers all R - register, I - immediate, and J - jump for the multicycle datapath.
4. All submodules are integrated into the main module.
5. The control state is based on the Mealy state machine.
6. As not all control signals are generated at any stage of datapath, it uses less power.
7. ALU has the dual function to cater its own job along with completing the job of the next address block of singlecycle datapath.

<table align="center">
  <tr>
    <th><h2><b>Pros</b></h2></th>
    <th><h2><b>Cons</b></h2></th>
  </tr>
  <tr>
    <td>Executes multiple instructions in a single clock cycle</td>
    <td>Complex to design.
  <tr>
    <td>Less Delay</td>
    <td>No parallel processing is available.</td>
  </tr>
  <tr>
    <td>Improved Performance of execution</td>
    <td>If the clock rate is increased by the same as the number of execution of instructions then performance is the same as the performance of singlecycle datapath.</td>
  </tr>
  <tr>
    <td>Covers almost all MiniMIPS instructions</td>
    <td>Complex to design ALU.</td>
  </tr>
  <tr>
    <td>Have numerous storage registers at each stage</td>
    <td>More numbers of registers, memory, and  2x1 mux are required.</td>
  </tr>
  <tr>
    <td>Less power consumption</td>
    <td>Calculation control signal generation at every stage is needed and so state machine design is also required. </td>
  </tr>
</table>

## **Key Skills-**

- ➤ Verilog HDL language 
- ➤ Computer Architecture
- ➤ Datapath performance management
- ➤ Fundamentals of Digital logic circuits
- ➤ Quartus IIModelsim Altera 
  




