# building tensorflow notes

This is *very* draft, work in progress :-P

First step is to compile one single tensorflow cuda file, eg cwise_op_gpu_add.cu.cc, into llvm IR.  ~~This doc is working on this bit for now.~~  This bit is done, in draft.  I had to hack in
a `using namespace std;`, and change gpu architecture to sm30, and then it worked ok.

Run:

[tensorflow/build_cwise_add.sh](https://github.com/hughperkins/cuda-ir-to-opencl/tree/master/tensorflow/build_cwise_add.sh)
