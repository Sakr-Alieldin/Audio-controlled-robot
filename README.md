# Audio-controlled-robot
This project implements a mobile robot controlled by audio commands using sound waves. Commands are transmitted via FSK modulation (800–1200 Hz) and decoded on-board using digital correlation running on a dsPIC33FJ128MC802 microcontroller.

The system is built around three main blocks:

Analog acquisition chain: microphone pre-amplification, band-pass filtering, and analog signal conditioning for ADC acquisition in low-SNR environments

Audio communication: binary FSK demodulation with chirp-based preamble detection and adaptive thresholding for robust synchronization

Motion control: closed-loop polar regulation using wheel encoders, trapezoidal velocity profiles, and PWM motor control for accurate translation and rotation

The robot reliably executes movement commands in noisy environments, achieving < 4% positioning error and robust operation up to ~2 m (and beyond in ideal conditions).
This project combines analog electronics, digital signal processing, embedded programming, and control systems into a fully functional prototype.
