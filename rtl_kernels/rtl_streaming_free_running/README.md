Stream Free Running
======================

This is a simple Vector Increment RTL Kernel design with 1 Stream input and 1 Stream output that demonstrates on how to process an input stream of data for computation in an application.

***KEY CONCEPTS:*** Read/Write Stream, Create/Release Stream, RTL Kernel

***KEYWORDS:*** cl_stream, CL_STREAM_EOT

## SUPPORTED PLATFORMS
Platform | Board             | Software Version
---------|-------------------|-----------------
xilinx_u200_qdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u250_qdma|Xilinx Alveo U250|VITIS 2019.2


##  DESIGN FILES
Application code is located in the src directory. Accelerator binary files will be compiled to the xclbin directory. The xclbin directory is required by the Makefile and its contents will be filled during compilation. A listing of all the files in this example is shown below

```
src/gen_xo.tcl
src/host.cpp
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./vadd_stream <myadder1 XCLBIN>
```

