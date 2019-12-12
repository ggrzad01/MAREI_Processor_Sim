# MAREI_Processor_Sim
A working design/simulation of the Machine Architecture that's Really Intuitive and Easy (MARIE) processor

The '.circ' requires Logisim to be opened.

test_programs/ includes .txt versions of test programs loaded into the processor RAM

This version of MARIE only includes the opcodes for Load, Store, Add, Subt, Input, Output, Halt, Skipcon, Jump, and Clear.

In the control unit, you can see that I tried to keep things as organized as possible. Each named OR gate at the top represents one micro operation eg: AC<-MBR. Instead of using arrows, "<-" I opted to use "<" because it fit within the OR gate outline much better. You can also see that I made use of D flip-flops when a demultiplexer would have worked just as well. This was for readability during testing. The poke tool gets exhausting to use after a while, so D flip-flops were the lazy way of displaying the binary opcode values.