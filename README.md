Speech Enhancement Using MATLAB

Overview
Speech Enhancement using MATLAB is a digital signal processing project that improves speech quality by reducing Gaussian noise using the spectral subtraction technique. It compares the original, noisy, and enhanced speech signals using time-domain waveforms, frequency spectra, and spectrograms.

 Objectives
- Add Gaussian noise to an original speech signal.
- Apply spectral subtraction for noise reduction.
- Analyze speech signals in the time and frequency domains.
- Compare original, noisy, and enhanced speech.
- Play and save the enhanced audio output.

 Technologies Used
- **Software:** MATLAB
- **Concepts:** Digital Signal Processing (DSP), FFT, Gaussian Noise, Spectral Subtraction
- **Audio Format:** WAV

 Project Workflow
1. Read the input speech audio file (`speech.wav`).
2. Convert stereo audio into mono, if required.
3. Add Gaussian noise to simulate a noisy environment.
4. Compute the FFT and estimate the noise spectrum.
5. Apply spectral subtraction and remove negative magnitude values.
6. Reconstruct the enhanced signal using the inverse FFT.
7. Normalize the output audio.
8. Plot waveforms, frequency spectra, and spectrograms.
9. Play and save the enhanced speech as `EnhancedSpeech.wav`.

Requirements
- MATLAB installed on your computer.
- An input speech audio file named `speech.wav`.
- MATLAB Signal Processing Toolbox may be required for the spectrogram function, depending on your MATLAB version.

How to Run
1. Clone or download this repository.
2. Place `speech.wav` in the same folder as the MATLAB script.
3. Open MATLAB and set the current folder to the project directory.
4. Run the MATLAB script.
5. Listen to the original, noisy, and enhanced speech.
6. View the generated plots and find `EnhancedSpeech.wav` in the project folder.

Expected Results
The project generates:
- Original speech waveform and frequency spectrum.
- Noisy speech waveform and frequency spectrum.
- Enhanced speech waveform and frequency spectrum.
- Spectrogram comparisons of all three signals.
- An enhanced audio file saved as `EnhancedSpeech.wav`.

Key Concepts
- **FFT:** Converts a time-domain signal into its frequency-domain representation.
- **Gaussian Noise:** Random noise added to simulate disturbances in speech.
- **Spectral Subtraction:** Reduces estimated noise components from the noisy signal's magnitude spectrum.
- **Inverse FFT:** Reconstructs the time-domain signal from the modified spectrum.

Limitations
This is a basic demonstration of spectral subtraction. Since the script uses the exact noise signal generated during simulation, it assumes the noise is known. In real-world applications, noise must be estimated from the noisy recording. The method may also introduce distortion or musical noise.

Future Improvements
- Estimate noise from silent portions of speech.
- Implement Wiener filtering.
- Compare Signal-to-Noise Ratio (SNR) before and after enhancement.
- Develop a MATLAB GUI for interactive speech enhancement.
- Test with real-world recordings containing background noise.

 Author
**Devika S. Nair**

---

⭐ If you find this project useful, consider giving the repository a star!
