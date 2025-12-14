AIM:

To implement JK flipflop using verilog and validating their functionality using their functional tables

SOFTWARE REQUIRED:

Quartus prime

THEORY

JK Flip-Flop

JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.
<img width="561" height="360" alt="Screenshot 2025-12-14 145922" src="https://github.com/user-attachments/assets/603c12fb-498a-45b2-bec8-3c9402834c6e" />


This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

<img width="440" height="335" alt="Screenshot 2025-12-14 145938" src="https://github.com/user-attachments/assets/805d0898-2229-4d8b-9877-6389e42e2369" />

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State

<img width="603" height="491" alt="Screenshot 2025-12-14 145950" src="https://github.com/user-attachments/assets/2b6be52a-0dfa-49ee-8104-bda0871ba199" />

By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

<img width="410" height="250" alt="Screenshot 2025-12-14 150009" src="https://github.com/user-attachments/assets/4c2eb4a6-93e1-4e39-af45-e4723acee01e" />

The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

Procedure

Identify present state 𝑄 𝑛 Q n​

Check inputs J and K

Wait for active clock edge

Apply JK rules (Set, Reset, Toggle, No change)

Determine next state 𝑄 𝑛

1 Q n+1​

PROGRAM

/* Program for flipflops and verify its truth table in quartus using Verilog programming. Developed by:YUVASREE S

RegisterNumber:25014012 */

RTL LOGIC FOR FLIPFLOPS

TIMING DIGRAMS FOR FLIP FLOPS

RESULTS: Thus the JK flipflop using verilog and validating their functionality using their functional tables is implemented and verified.
