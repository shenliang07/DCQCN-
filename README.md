# DCQCN-
NS-3 simulator for RDMA

This is an NS-3 simulator for RDMA over Converged Ethernet v2 (RoCEv2). It includes the implementation of DCQCN, TIMELY, PFC, ECN and Broadcom shared buffer switch.

It is based on NS-3 version 3.17, and ported to Visual Studio environment, as explained here.
Source code comes from https://github.com/bobzhuyb/ns3-rdma

Note

TIMELY implementation is in "timely" branch and hasn't been merged into the master branch. So, you may not be able to simulate DCQCN and TIMELY simultaneously at this moment.

Quick Start

Build

To compile it out-of-the-box, you need Visual Studio 2015 (not 2013 or 2017). People have successfully built it with free version, which can be downloaded here. Open windows/ns-3-dev/ns-3-dev.sln, just build the whole solution.

If you cannot get a Windows machine or Visual Studio for any reason, you may try building it with the original Makefile. We have done it a while back, but now you probably need to edit a few things in waf to make it work.

Run

The binary will be generated at windows/ns-3-dev/x64/Release/main.exe. We include a sample configuration file at windows/ns-3-dev/x64/Release/mix/config.txt Execute main.exe in windows/ns-3-dev/x64/Release/:

cd windows\ns-3-dev\x64\Release\
main.exe mix\config.txt
