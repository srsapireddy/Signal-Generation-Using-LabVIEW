# Signal Generation Using LabVIEW

This repository contains simple AM and FM signal generation experiments using LabVIEW.

---

# AM Signal Generation in LabVIEW

This project shows a simple Amplitude Modulation (AM) signal generated using LabVIEW.

The experiment includes:

- Message signal
- Carrier signal
- AM modulated signal
- Filtered output signal

## Block Diagram

<img width="1696" height="894" alt="AM Block Diagram" src="https://github.com/user-attachments/assets/f903a45d-a69e-4eab-9c8e-acef1a001071"/>

## Front Panel Output

<img width="1585" height="827" alt="AM Front Panel Output" src="https://github.com/user-attachments/assets/7dbc7833-297c-4c0c-940e-49bf04b4351b"/>

## Description

Amplitude Modulation changes the amplitude of a high-frequency carrier signal according to the message signal.

AM equation:

s(t) = Ac [1 + m(t)] cos(2πfc t)

where:

- s(t) is the AM signal
- Ac is the carrier amplitude
- m(t) is the message signal
- fc is the carrier frequency

## AM Signal Flow

<img width="1448" height="1086" alt="AM Signal Flow Diagram" src="https://github.com/user-attachments/assets/bd5752bc-dfd8-4a09-b96a-ac147dedfe7b" />

## Result

The AM signal was successfully generated and displayed using LabVIEW.

---

# FM Signal Generation in LabVIEW

This project shows a simple Frequency Modulation (FM) signal generated using LabVIEW.

The experiment includes:

- Message signal
- Cosine carrier signal
- Sine carrier signal
- FM modulated signal

## Block Diagram

<img width="1197" height="956" alt="FM Block Diagram" src="https://github.com/user-attachments/assets/19983b2f-7936-4a0b-9fa9-15ab2e7eb891" />

## Front Panel Output

<img width="1220" height="812" alt="FM Front Panel Output" src="https://github.com/user-attachments/assets/03f539c9-348e-47fd-91bd-5ff25832c354" />

## Description

Frequency Modulation changes the frequency of a carrier signal according to the message signal. In FM, the carrier amplitude remains almost constant, but the frequency changes based on the message signal.

FM equation:

s(t) = Ac cos(2πfc t + beta sin(2πfm t))

where:

- s(t) is the FM signal
- Ac is the carrier amplitude
- fc is the carrier frequency
- fm is the message frequency
- beta is the modulation index

## Result

The FM signal was successfully generated and displayed using LabVIEW.

---

## Software Used

- LabVIEW
