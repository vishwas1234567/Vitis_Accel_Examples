Adder With Streams (RTL)
======================

This example shows an adder with streams using 3 RTL kernels.

***KEY CONCEPTS:*** RTL Kernel, Multiple RTL Kernels

## SUPPORTED PLATFORMS
Platform | Board             | Software Version
---------|-------------------|-----------------
xilinx_u200_qdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u200_xdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u250_qdma|Xilinx Alveo U250|VITIS 2019.2
xilinx_u250_xdma|Xilinx Alveo U250|VITIS 2019.2
xilinx_u280_xdma|Xilinx Alveo U280|VITIS 2019.2
xilinx_u50_xdma|Xilinx Alveo U50|VITIS 2019.2
zc702_base|Xilinx Zynq-7000 SoC ZC702|VITIS 2019.2
zc706_base|Xilinx Zynq-7000 SoC ZC706|VITIS 2019.2
zcu102_base|Xilinx UltraScale+ MPSoC ZCU102|VITIS 2019.2
zcu104_base|Xilinx UltraScale+ MPSoC ZCU104|VITIS 2019.2


##  DESIGN FILES
Application code is located in the src directory. Accelerator binary files will be compiled to the xclbin directory. The xclbin directory is required by the Makefile and its contents will be filled during compilation. A listing of all the files in this example is shown below

```
src/host.cpp
src/ip/ip_1/component.xml
src/ip/ip_1/src/krnl_input_stage_rtl.v
src/ip/ip_1/src/krnl_input_stage_rtl_axi_read_master.sv
src/ip/ip_1/src/krnl_input_stage_rtl_control_s_axi.v
src/ip/ip_1/src/krnl_input_stage_rtl_counter.sv
src/ip/ip_1/src/krnl_input_stage_rtl_int.sv
src/ip/ip_1/xgui/krnl_input_stage_rtl_v1_0.tcl
src/ip/ip_2/component.xml
src/ip/ip_2/src/krnl_adder_stage_rtl.v
src/ip/ip_2/src/krnl_adder_stage_rtl_adder.sv
src/ip/ip_2/src/krnl_adder_stage_rtl_control_s_axi.v
src/ip/ip_2/src/krnl_adder_stage_rtl_counter.sv
src/ip/ip_2/src/krnl_adder_stage_rtl_int.sv
src/ip/ip_2/xgui/krnl_adder_stage_rtl_v1_0.tcl
src/ip/ip_3/component.xml
src/ip/ip_3/src/krnl_output_stage_rtl.v
src/ip/ip_3/src/krnl_output_stage_rtl_axi_write_master.sv
src/ip/ip_3/src/krnl_output_stage_rtl_control_s_axi.v
src/ip/ip_3/src/krnl_output_stage_rtl_counter.sv
src/ip/ip_3/src/krnl_output_stage_rtl_int.sv
src/ip/ip_3/src/krnl_output_stage_rtl_register_slice.sv
src/ip/ip_3/xgui/krnl_output_stage_rtl_v1_0.tcl
src/kernel_adder_stage.xml
src/kernel_input_stage.xml
src/kernel_output_stage.xml
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./host <adder XCLBIN>
```

