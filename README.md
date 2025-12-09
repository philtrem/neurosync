# NeuroSync v4.9

A sophisticated brainwave entrainment tool that combines binaural beats, visual strobing, and ambient noise to help achieve various mental states such as deep focus, relaxation, or meditation.

## Features

### Audio Entrainment
- **Binaural Beats**: Generate precise binaural beats using independent left/right carrier frequencies
- **Customizable Parameters**:
  - Target brainwave frequency (1-50 Hz)
  - Carrier frequency (100-800 Hz)
  - Beat intensity (0-100%)
  - Master volume control (0-100%)
- **Multiple Noise Types**:
  - AM Noise (Amplitude Modulated)
  - Pink Noise
  - White Noise
  - Brown Noise

### Visual Strobing
- **Monitor-Synchronized Flashing**: Visual strobe that syncs with your monitor's refresh rate
- **Smart Jitter Detection**: Automatically calculates and warns about timing mismatches
- **Customizable**:
  - Strobe color picker
  - Brightness control (0-100%)
  - Enable/disable toggle
- **Jitter Analysis**: Real-time feedback on sync quality (perfect sync, micro-jitter, or heavy jitter)

### User Experience
- **Day/Night Profiles**: Two separate profiles with different color schemes and saved settings
- **Collapsible Interface**: Minimize the UI during sessions for distraction-free use
- **Frequency Scanning**: Quick increment/decrement buttons for brainwave frequency
- **Performance Monitoring**: Optional FPS counter and frame drop detection
- **Auto-Save**: Settings are automatically saved to localStorage
- **Monitor Refresh Detection**: Automatic detection of your display's refresh rate

### Technical Capabilities
- Precise frequency generation using Web Audio API
- Real-time performance metrics and dropped frame detection
- Monitor refresh rate synchronization for smooth visual effects

## Getting Started

### Installation
1. Download or clone the `neurosync.html` file
2. Open it in a modern web browser (Chrome, Firefox, Edge, or Safari)
3. Grant audio permissions when prompted
4. Start your session!

### Basic Usage
1. **Adjust Parameters**: Use the sliders to set your desired brainwave frequency, carrier frequency, and other parameters
2. **Enable Strobing** (optional): Toggle the visual strobe and adjust color/brightness
3. **Choose Noise Type**: Select your preferred ambient noise (or AM for modulated tones)
4. **Start Session**: Click the "Start Session" button to begin
5. **Monitor Feedback**: Watch for jitter warnings if using strobing

### Recommended Settings

#### Deep Focus (Beta Waves)
- Brainwave: 14-30 Hz
- Carrier: 200-300 Hz
- Beat Intensity: 60-80%
- Strobe: Optional

#### Relaxation (Alpha Waves)
- Brainwave: 8-13 Hz
- Carrier: 150-250 Hz
- Beat Intensity: 40-60%
- Strobe: Disabled or low brightness

#### Meditation (Theta Waves)
- Brainwave: 4-7 Hz
- Carrier: 100-200 Hz
- Beat Intensity: 30-50%
- Strobe: Disabled

#### Deep Sleep (Delta Waves)
- Brainwave: 0.5-3 Hz
- Carrier: 100-150 Hz
- Beat Intensity: 20-40%
- Strobe: Disabled

## Technical Details

### Brainwave Frequency Ranges
- **Delta (0.5-4 Hz)**: Deep sleep, healing
- **Theta (4-8 Hz)**: Meditation, creativity, REM sleep
- **Alpha (8-13 Hz)**: Relaxation, pre-sleep, light meditation
- **Beta (13-30 Hz)**: Alert, focused, active thinking
- **Gamma (30-50 Hz)**: High-level cognitive processing

### Audio Engine
- Built with Web Audio API for precise frequency control
- Stereo panning for true binaural beat generation
- Multiple oscillator types for rich sound design
- Real-time noise generation and filtering

### Visual Strobing
The visual strobe feature uses `requestAnimationFrame` synchronized with your monitor's refresh rate. The jitter detection system calculates timing precision:
- **Perfect Sync** (< 0.005 difference): Optimal timing
- **Micro-Jitter** (< 0.2 difference): Minor timing variations
- **Heavy Jitter** (> 0.2 difference): Significant timing mismatch

### Data Persistence
Settings are saved to browser localStorage:
- `neurosync_day`: Day profile settings
- `neurosync_night`: Night profile settings
- `neurosync_last_mode`: Last used profile

## Browser Compatibility
- ✅ Chrome/Edge (Recommended)
- ✅ Firefox
- ✅ Safari
- ⚠️ Requires modern browser with Web Audio API support

## Safety Warnings

### ⚠️ IMPORTANT - READ BEFORE USE

**DO NOT USE if you have:**
- Epilepsy or history of seizures
- Photosensitive conditions
- Any seizure-related medical conditions

**Visual Strobing:**
- The strobe feature may trigger seizures in people with photosensitive epilepsy
- Use at your own risk and start with low brightness
- Discontinue immediately if you experience dizziness, discomfort, or visual disturbances

**Audio Safety:**
- Keep volume at comfortable levels
- Take breaks every 30-60 minutes
- Do not use while driving or operating machinery

**General:**
- This tool is for experimental/entertainment purposes only
- Not a medical device or treatment
- Consult a healthcare professional before use if you have any concerns

## Keyboard Shortcuts
- None currently implemented (use UI controls)

## Profile Management
- **Day Profile**: Default blue/teal color scheme
- **Night Profile**: Warm orange/brown color scheme optimized for low-light use
- **Switch Profiles**: Click the moon/sun icon in the header
- **Reset Profile**: Use the "Reset Profile" button to restore defaults

## Tips for Best Results
1. Use headphones for optimal binaural beat experience
2. Find a quiet, comfortable environment
3. Keep strobe brightness low initially
4. Experiment with different frequencies for different goals
5. Use the auto-detect feature to find your monitor's refresh rate
6. Pay attention to jitter warnings when using strobing
7. Start with shorter sessions (10-15 minutes) and gradually increase

## Troubleshooting

### No Sound
- Check browser audio permissions
- Ensure volume sliders are not at 0
- Try refreshing the page and starting again

### Strobing Not Working
- Ensure strobe toggle is enabled
- Check brightness setting
- Verify monitor refresh rate is detected correctly

### Heavy Jitter Warning
- Try the suggested frequency from the warning message
- Use the "Detect" button to accurately measure your refresh rate
- Consider disabling strobe if jitter cannot be resolved

### Performance Issues
- Disable FPS display if not needed
- Close other browser tabs
- Use a more powerful device

## Technical Specifications
- **File Size**: ~30KB (single HTML file)
- **Dependencies**: None (vanilla JavaScript)
- **Audio Latency**: < 10ms (browser dependent)
- **Visual Refresh**: Up to 240Hz (monitor dependent)

## Version History
- **v4.9**: AM Noise Fix - Current version with improved amplitude modulation

## Contributing
N.B.: please only submit bug fixes

This is a single-file web application. To contribute:
1. Fork the repository
2. Make your changes to `neurosync.html`
3. Test thoroughly across different browsers
4. Submit a pull request with a clear description

## License
[Specify your license here - e.g., MIT, GPL, etc.]

## Disclaimer
NeuroSync is provided "as is" without warranty of any kind. The authors are not responsible for any effects, adverse or otherwise, that may result from using this tool. Use at your own risk.

## Credits
Developed with Web Audio API and modern web technologies.

---

**Remember**: Start slow, use responsibly, and listen to your body. If something doesn't feel right, stop immediately.