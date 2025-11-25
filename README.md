# DSB--SC-MODULATION-AND-DEMODULATION-USING-PYTHON

__AIM__:

To generate a Double Sideband Suppressed Carrier (DSB-SC) signal in Python (Google Colab), transmit it (optionally add noise), and recover the message using coherent (synchronous) demodulation with a low-pass filter. Observe time and frequency domain waveforms and measure demodulation performance

__APPARATUS REQUIRED__:

Google Colab (or any Python environment)

Python libraries: numpy, matplotlib, scipy (scipy.signal)

__Theory__:

DSB-SC signal: s(t) = m(t) · cos(2πf_c t)
Coherent demodulation: multiply received s(t) by a synchronized carrier cos(2πf_c t) then low-pass filter (LPF) to remove double-frequency components:

r(t) = s(t)·cos(2πf_c t) = m(t)·cos²(2πf_c t) = 0.5 m(t) + 0.5 m(t)·cos(4πf_c t)
LPF extracts 0.5·m(t) → scale by 2 to recover m(t).

__Procedure__:

1) Import libraries and set parameters
2) Define message and carrier signals
3) Generate DSB-SC signal (modulation)
4) View spectra (FFT) of message and DSB-SC
5) (Optional) Add noise
6) Coherent demodulation (multiply by synchronized carrier)
7) Low-pass filter to recover message

   __Tabulation__:
![WhatsApp Image 2025-11-26 at 00 13 16_5b6dd8fa](https://github.com/user-attachments/assets/6477c719-de16-470c-a2d3-99254cc74010)

   __Output__:
![WhatsApp Image 2025-11-26 at 00 15 10_e7a35835](https://github.com/user-attachments/assets/c6beeb46-4b28-46f0-801e-a974dcde9451)

   __Result__:
![WhatsApp Image 2025-11-26 at 00 13 23_c9253fa5](https://github.com/user-attachments/assets/c667baef-f095-4c16-903f-a491903bbc5e)
