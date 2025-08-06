

# FaceScrollController: Hands-Free Scrolling with Facial Recognition

![FaceScrollController Demo](https://img.shields.io/badge/Status-Active-brightgreen) ![Python](https://img.shields.io/badge/Python-3.6%2B-blue) ![License](https://img.shields.io/badge/License-MIT-green)

A revolutionary hands-free scrolling system that uses your webcam and facial recognition to control scrolling movements. Simply tilt your head up or down to scroll through content without touching your mouse or keyboard.

## Features

- **Hands-Free Operation**: Control scrolling with natural head movements
- **Real-Time Face Tracking**: Uses MediaPipe for accurate facial landmark detection
- **Visual Feedback**: See your face mesh and scroll direction indicators in real-time
- **Customizable Settings**: Adjust scroll sensitivity and amount to your preference
- **Health Benefits**: Helps tone jawline, neck, and platysma muscles while you work
- **Multi-Tasking Friendly**: Scroll while eating, writing, or doing other tasks

## How It Works

The application uses your computer's webcam to track facial landmarks, specifically monitoring the vertical position of your nose tip. When you move your face up or down beyond a set threshold, it triggers a scroll action in the corresponding direction.

1. **Face Detection**: MediaPipe Face Mesh detects your face and key landmarks
2. **Movement Tracking**: The vertical position of your nose tip is tracked frame by frame
3. **Scroll Trigger**: When your face moves up/down beyond the threshold, a scroll command is sent
4. **Visual Feedback**: The application shows your face mesh and scroll direction indicators

## Installation

### Prerequisites

- Python 3.6 or higher
- A working webcam
- OpenCV-compatible system

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/face-scroll-controller.git
   cd face-scroll-controller
   ```

2. Install the required packages:
   ```bash
   pip install opencv-python mediapipe pyautogui numpy
   ```

3. Run the application:
   ```bash
   python face_scroll_controller.py
   ```

## Usage

1. **Start the Application**: Run the script and position your face in the center of the frame.
2. **Activate Scrolling**: Press the SPACE key to enable scrolling.
3. **Control Scrolling**:
   - Tilt your head UP to scroll UP
   - Tilt your head DOWN to scroll DOWN
4. **Deactivate Scrolling**: Press SPACE again to pause scrolling.
5. **Exit**: Press ESC to close the application.

### Controls

| Key | Action |
|-----|--------|
| SPACE | Start/Stop scrolling |
| ESC | Exit application |

## Customization

You can adjust the following parameters in the `FaceScrollController` class:

- `scroll_threshold`: Minimum pixels of movement to trigger scrolling (default: 15)
- `scroll_amount`: Number of pixels to scroll per trigger (default: 85)
- `scroll_cooldown`: Seconds between scroll actions to prevent excessive scrolling (default: 0.1)

## Requirements

- Python 3.6+
- OpenCV (cv2)
- MediaPipe
- PyAutoGUI
- NumPy
- A working webcam

## Health Benefits

Regular upward head movements while using this application can help:
- Tone your jawline muscles
- Strengthen neck muscles
- Exercise the platysma muscles
- Reduce hand strain from repetitive scrolling

As we say in Malayalam, "ota veddik rand pakshi" - it's like getting a jawline workout while you work!

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [MediaPipe](https://google.github.io/mediapipe/) for the face mesh detection
- [OpenCV](https://opencv.org/) for computer vision capabilities
- [PyAutoGUI](https://pyautogui.readthedocs.io/) for scroll control



**Note**: This application uses your webcam only for local processing. No video data is transmitted or stored.
