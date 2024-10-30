# SounT

SounT is an audio processing system for real-time mixing, mastering, and splicing of audio tracks.
It supports multiple audio formats and dynamically adapts to listening devices and user preferences, ensuring a customized audio experience.
The tool comes with a RESTful API for easy integration with existing audio systems.

## Applications

I want to build this to be most generally applicable.<br>
I'm thinking of use cases like these that could be most helpful:

- General Audio production
- Live sound reinforcement
- Streaming platforms
- Augmented reality audio
- Hearing aid technology
- Automotive sound systems

## Roadmap

- [ ] Core Processing
  - [x] Basic audio file reading/writing functionality
  - [ ] Implement basic audio splicing models
  - [ ] Investigate usability of https://huggingface.co/datasets/jxie/musdb18
  - [ ] Real-time stream processing capability
  - [ ] Modules for mixing, mastering, and splicing
- [ ] AI Integration
  - [ ] Initial training setup for AI model for audio enhancement
  - [ ] Initial training setup for AI model for audio splicing
  - [ ] Implement device recognition
  - [ ] Initial setup for user preference learning mechanism
  - [ ] Implement device-adaptive EQ
  - [ ] Implement dynamic compression
- [ ] API Development
  - [ ] Design RESTful API architecture
  - [ ] Implement core API endpoints
- [ ] User Interface
  - [ ] Build Desktop UI with mobile app portability
  - [ ] Create web-based control panel

## Getting Started

For a start, this is what I want to get working:

```python
import sount

# Initialize SounT with default settings
processor = sount.AudioProcessor()

# Process an audio file
processed_audio = processor.process("input.wav", device="smartphone")

# Save the processed audio
processed_audio.save("output.wav")
```
