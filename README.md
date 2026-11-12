# Ear Trainer

Phone-friendly web app for learning frequencies by ear. Single file, no dependencies.

**Live:** https://briangooding.github.io/ear-trainer/ (microphone needs https)

- **Analyzer:** live spectrum (log frequency axis) plus a scrolling spectrogram, and a readout of the loudest frequency in Hz, nearest note, cents off and tonal band (bass, mids, presence...). Tap the spectrum to read any frequency.
- **Freeze:** holds the spectrum and drops an orange dot on the captured peak. Drag it (or touch anywhere on the spectrum) to play that frequency and match it to what you heard; "Play tone" holds it, "Back to captured peak" snaps back.
- **Tone:** play any 20 Hz–16 kHz tone (sine, triangle, square, saw) by slider, number, semitone/octave steps, or by tapping the spectrum. Landmark chips jump to useful frequencies.
- **Quiz:** *Learn* mode plays a frequency per button; *Test* mode plays a hidden tone and you name it (octave or ⅓-octave levels). Spectrum is hidden until you answer. Score and streak are saved on the device.

The mic is opened with echo cancellation, noise suppression and auto-gain off so tones aren't filtered. Peak frequency uses a 16384-point FFT with parabolic interpolation (about ±1 Hz).
