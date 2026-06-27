# Signal-Generation-Using-LabVIEW
# AM Signal Generation in LabVIEW

This project shows a simple Amplitude Modulation (AM) signal generated using LabVIEW.

The experiment includes:

- Message signal
- Carrier signal
- AM modulated signal
- Filtered output signal

## Block Diagram

<img width="1696" height="894" alt="image" src="https://github.com/user-attachments/assets/f903a45d-a69e-4eab-9c8e-acef1a001071" />

## Front Panel Output

<img width="1585" height="827" alt="image" src="https://github.com/user-attachments/assets/7dbc7833-297c-4c0c-940e-49bf04b4351b" />

## Description

Amplitude Modulation changes the amplitude of a high-frequency carrier signal according to the message signal.

The AM signal can be written as:

<img width="1448" height="1086" alt="image" src="https://github.com/user-attachments/assets/bd5752bc-dfd8-4a09-b96a-ac147dedfe7b" />

```math
s(t) = A_c[1 + m(t)]\cos(2\pi f_c t)
