# 🪙 Coin Toss App for Flipper Zero

A fun and interactive coin toss simulator for the Flipper Zero device. Flip a virtual coin and test your luck!

## 🎮 Features

- **Interactive Menu**: Choose between Heads or Tails
- **Animated Coin Flip**: Watch the coin spin with a progress bar
- **Random Results**: True 50/50 chance using hardware RTC
- **Win/Lose Feedback**: Clear indication of your success
- **Replay Function**: Play again or exit easily

## 📱 How to Play

1. **Select your guess**: Use Left/Right buttons to choose Heads or Tails
2. **Watch the flip**: Enjoy the spinning animation
3. **See the result**: Find out if you won or lost
4. **Play again**: Press OK to flip again, or Back to exit

## 🛠️ Installation

### Method 1: Manual Installation (Recommended)

1. **Clone this repository**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/flipper-coin-toss.git
   cd flipper-coin-toss
   ```

2. **Copy to Flipper Zero firmware**:
   ```bash
   # Navigate to your Flipper Zero firmware directory
   cd ~/flipperzero-firmware/applications/
   
   # Copy the app
   cp -r /path/to/flipper-coin-toss coin_toss
   ```

3. **Build and install**:
   ```bash
   # From the firmware root directory
   ./fbt fap_example_adc
   ./fbt launch_app APPSRC=applications/coin_toss
   ```

### Method 2: Using Flipper Zero App Manager

1. Download the `.fap` file from releases
2. Use the Flipper Zero App Manager to install
3. The app will appear in Apps → Examples → example_adc

## 🔧 Development

### Building from Source

```bash
# Navigate to Flipper Zero firmware
cd ~/flipperzero-firmware

# Build the app
./fbt fap_example_adc

# Launch on device
./fbt launch_app APPSRC=applications/coin_toss
```

### Project Structure

```
coin_toss/
├── example_adc.c      # Main application code
├── application.fam    # App manifest
├── CMakeLists.txt     # Build configuration
└── README.md         # This file
```

## 🎯 Controls

- **Left Button**: Select Heads
- **Right Button**: Select Tails
- **OK Button**: Confirm selection / Play again
- **Back Button**: Exit app

## 📋 Requirements

- Flipper Zero device
- Flipper Zero firmware (latest version recommended)
- USB connection for installation

## 🤝 Contributing

Feel free to submit issues, feature requests, or pull requests!

## 📄 License

This project is open source. Feel free to modify and distribute.

## 🙏 Credits

Created for the Flipper Zero community. Enjoy flipping coins! 🪙 