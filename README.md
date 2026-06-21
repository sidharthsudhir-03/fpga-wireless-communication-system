# FPGA Wireless Communication System

FPGA implementation of a reliable wireless audio communication system on the Intel DE1-SoC platform. The system performs audio acquisition, error correction encoding, QPSK modulation, pulse shaping, channel transmission, reception, demodulation, and audio reconstruction.

---

## Overview

This project was developed as part of a three-person team project focused on the reliable transmission of audio data over a noisy wireless channel. The design was implemented and verified using MATLAB/Simulink, ModelSim, and Verilog/SystemVerilog, with deployment on the Intel DE1-SoC FPGA platform.

The communication chain includes ADC/DAC conversion, convolutional encoding, QPSK modulation, raised cosine pulse shaping, Gilbert fading/AWGN channel modeling, matched filtering, demodulation, and Viterbi decoding.

---

## My Contributions

As part of a three-person team, I was responsible for:

- FPGA transmitter implementation
- FPGA receiver implementation
- Gilbert fading channel model implementation
- Oversampling and interpolation for channel transmission
- Downsampling and symbol recovery at the receiver
- FPGA integration, debugging, and verification

---

## System Architecture

```text
Audio Source
     │
     ▼
ADC
     │
     ▼
Convolutional Encoder
     │
     ▼
QPSK Modulator
     │
     ▼
Raised Cosine Transmit Filter
     │
     ▼
Gilbert Fading / AWGN Channel
     │
     ▼
Raised Cosine Receive Filter
     │
     ▼
QPSK Demodulator
     │
     ▼
Viterbi Decoder
     │
     ▼
DAC
     │
     ▼
Audio Output
```

---

## Key Features

- Reliable wireless audio transmission
- Gray-coded QPSK modulation and demodulation
- Convolutional error correction encoding
- Viterbi decoding
- Raised cosine pulse shaping and matched filtering
- Gilbert fading channel model
- FPGA implementation on Intel DE1-SoC
- MATLAB/Simulink system validation
- Verilog/SystemVerilog hardware implementation

---

## Performance

| Metric | Value |
|----------|----------|
| Platform | Intel DE1-SoC FPGA |
| Message Bandwidth | 8 kHz |
| Channel Sample Rate | 1 MHz |
| Channel Bandwidth | 100 kHz |
| Modulation Scheme | QPSK |
| Target BER | 1×10⁻⁴ |
| Simulated BER | 0 – 5×10⁻⁵ |
| FPGA Processing Delay | 0.29 ms |

---

## Technologies Used

- Verilog
- SystemVerilog
- MATLAB
- Simulink
- ModelSim
- Intel Quartus
- Intel DE1-SoC FPGA

---

## Repository Structure

```text
rtl/
├── FPGA source files

matlab/
├── MATLAB analysis scripts
├── Simulink models

reports/
├── Final project report

demo/
├── Demonstration material
```

---

## Learning Outcomes

- Digital communication systems
- FPGA-based signal processing
- Digital modulation and demodulation
- Error correction coding
- Pulse shaping and matched filtering
- Channel modeling
- RTL design and verification
- FPGA system integration
