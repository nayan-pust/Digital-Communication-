# Digital-Communication-
Digital Communication || Signal Shifting || ASK || FSK || Analog Signal Transfer 
****
# **Have Some Basic problem List to Signal Shifting Analysis**
```ruby 1. MATLAB program for Uni-polar Non-Return to Zero (NRZ) Line Coding.
2. MATLAB program for Polar Non-Return to Zero (NRZ) Line Coding.
3. MATLAB program for Uni-polar Return to Zero (RZ) Line Coding.
4. MATLAB program for Bi-polar Return to Zero (RZ) Line Coding.
5. MATLAB program for Split-Phase (Manchester Code).
6. MATLAB program for binary Amplitude Shift Keying (ASK) Modulation and Demodulation.
7. MATLAB program for Frequency Shift Keying (FSK) Modulation and Demodulation.
8. MATLAB program for Phase Shift Keying (PSK) Modulation and Demodulation.
9. MATLAB program for Quadrature Phase Shift Keying (QPSK) Modulation and Demodulation.
10. MATLAB program for Pulse Amplitude Modulation (PAM) and Demodulation.
```
**Line Coding: Refers to the information data/digital data / numerical data convert into transmittable form that means convert waveform**
![image](https://github.com/nayan-pust/Digital-Communication-/assets/114688354/96d58152-e668-4c07-be56-04944e8676df)
![image](https://github.com/nayan-pust/Digital-Communication-/assets/114688354/c99f2b11-f18a-4a36-8df3-828580aff521)

```ruby
Here RZ means Return Zero.
NRZ means Non Return Zero.
```
# Ploting Explain 
![image](https://github.com/nayan-pust/Digital-Communication-/assets/114688354/1e4907ac-2716-49a0-b276-d3bc651401f0)
```ruby
A1 = 10
A2 = 5
br = 1 / bp
f = br * 10
t2 = np.arange(bp / 99, bp + bp/99, bp / 99)
ss = len(t2)
m = np.array([])
for i in range(len(x)):
    if x[i] == 1:
        y = A1 * np.cos(2 * np.pi * f * t2)
    else:
        y = A2 * np.cos(2 * np.pi * f * t2)
    m = np.concatenate((m, y))

t3 = np.arange(bp / 99, bp * len(x), bp / 99)
plt.subplot(312)
plt.plot(t3, m)
plt.grid(True)
plt.xlabel("Time (sec)")
plt.ylabel("Amplitude (volt)")
plt.title("Waveform for binary ASK Modulation Corresponding Binary Information")
```
# Explain 
```ruby
A1 = 10
A2 = 5
**A1 represents the high amplitude level, and A2 represents the low amplitude level.**
```
