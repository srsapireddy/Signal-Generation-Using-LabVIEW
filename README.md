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

# PM Signal Generation in LabVIEW

This project shows a simple Phase Modulation (PM) signal generated using LabVIEW.

The experiment includes:

- Message signal
- Cosine carrier signal
- Sine carrier signal
- Phase modulated signal
- PM result waveform

## Block Diagram

<img width="1516" height="863" alt="image" src="https://github.com/user-attachments/assets/5bb1e483-0835-4e18-90b3-a9347d374d0f" />

## Front Panel Output

<img width="1471" height="797" alt="image" src="https://github.com/user-attachments/assets/f288bbd9-f7e4-4463-a06d-9a8130ed2266" />

## Description

Phase Modulation changes the phase of the carrier signal according to the message signal.

In PM, the amplitude of the carrier remains almost constant, but the phase shifts based on the message signal.

PM equation:

s(t) = Ac cos(2πfc t + kp m(t))

where:

- s(t) is the PM signal
- Ac is the carrier amplitude
- fc is the carrier frequency
- kp is the phase sensitivity
- m(t) is the message signal

If the message signal is:

m(t) = sin(2πfm t)

then the PM signal is:

s(t) = Ac cos(2πfc t + kp sin(2πfm t))

## LabVIEW Implementation

In this LabVIEW design, the message signal is used to control the phase of the carrier signal.

The cosine carrier and sine carrier components are combined with the message signal to generate the PM waveform. The final phase modulated signal is displayed using the PM Result waveform graph.

## Result

The PM signal was successfully generated and displayed using LabVIEW.

# ASK Signal Generation Using LabVIEW

## Amplitude Shift Keying (ASK) Signal Generation in LabVIEW

This project demonstrates the generation of an **Amplitude Shift Keying (ASK)** signal using LabVIEW.

ASK is a digital modulation technique where the amplitude of the carrier signal changes according to the binary input data.

In this project:

- Binary input data is generated
- A carrier signal is generated
- The carrier is transmitted when the binary bit is `1`
- The carrier is turned off when the binary bit is `0`
- The ASK modulated waveform is displayed on the waveform chart

---

## Block Diagram

The LabVIEW block diagram shows the implementation of ASK modulation.

The binary data is generated using random values and compared with a threshold value.  
Based on the binary value, the carrier signal is either passed or suppressed.

<img width="1888" height="905" alt="image" src="https://github.com/user-attachments/assets/2d84ef24-9497-48ac-8647-eb1dd7873c5a" />

---

## Front Panel Output

The front panel shows the generated ASK signal and the corresponding digital binary signal.

<img width="1878" height="970" alt="image" src="https://github.com/user-attachments/assets/b2e728b9-64a6-4f81-b892-ba085c61e26f" />

---

## Working Principle

Amplitude Shift Keying changes the amplitude of the carrier signal based on the binary input.

For binary `1`, the carrier signal is present.

For binary `0`, the carrier signal is absent.

The ASK signal can be written as:

```text
ASK Signal = m(t) × Carrier Signal
