Error Handling (CPP)
======================

This example discuss the different reasons for errors in OpenCL C++ and how to handle them at runtime.

***KEY CONCEPTS:*** OpenCL C++ API, Error handling

***KEYWORDS:*** CL_SUCCESS, CL_DEVICE_NOT_FOUND, CL_DEVICE_NOT_AVAILABLE, CL_INVALID_VALUE, CL_INVALID_KERNEL_NAME, CL_INVALID_BUFFER_SIZE

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
src/vector_addition.cpp
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./errors <vector_addition XCLBIN>
```

