# Mac-Ops
A script to optimize your macOS system for live performances or resource-intensive processing. It disables unnecessary services (Wi-Fi, Bluetooth, Spotlight, Notifications, etc.), purges caches, and frees up resources to improve performance stablity. Revert to previous system settings with one click.

Originally designed to stabilize and boost the performance of mature MacOS systems, this is a handy app to simplify pre-show system tuning. Benchmarked with a MacBook Pro 2015, MacOS Catalina for live audio performance. Script developed with assistance from DeepSeek-V3 

---

## Features
- **Optimize:** Disables Wi-Fi, Bluetooth, Spotlight indexing, notifications, and graphics effects, and clears caches.
- **Revert:** Restores all settings to their original state.
- **Legacy Support** Automatically detects missing elements from older configurations with the option to skip. Added support for detections of `blueutil` for Bluetooth control (installed by default with MacOS Big Sur and after).
- **User-Friendly:** Simple GUI with options to optimize, revert, or quit. Easy to add additional variables for further customization.

---

## Requirements
- macOS (tested on Catalina and later).
- `blueutil` (optional, for Bluetooth control). Install it via Homebrew:
  ```bash
  brew install blueutil
  ```

---

## Installation
1. Download the script or clone the repository.
2. Open the script in **Script Editor** on macOS.
3. Save the script as an application:
   - Go to **File > Save**.
   - Set the **File Format** to **Application**.
   - Choose a location to save the app (e.g., Desktop).

---

## Usage
1. Double-click the app to launch it.
2. Choose **Optimize** to apply performance optimizations.
3. Return your system to its original state, choose **Revert** to restore your system to its original state.

---

## Script Details
The script uses AppleScript and shell commands to:
- Disable/enable Wi-Fi (`networksetup`).
- Disable/enable Bluetooth (`blueutil`).
- Disable/enable Spotlight indexing (`mdutil`).
- Disable/enable notifications (`defaults` and `killall`).
- Reduce graphics effects (`defaults`).
- Clear caches (`purge`).
- Add custom commands easily with a script editor.

---

## Credits
- Author: **LLPPR** (https://github.com/LLPPR)
- Co-Author: **DeepSeek "Rock On" V3**

---

## License
This project is licensed under the MIT License. Feel free to use, modify, and share it!
