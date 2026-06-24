LIEF for Termux & Pydroid3

Python 3.13 Compatible Library for Mobile/ARM Environments

This project is a mobile-optimized distribution of the LIEF (Library to Instrument Executable Formats) library, specifically built for:

· Termux (Android terminal emulator)
· Pydroid3 (Android Python IDE)

📌 Important Note

This repository contains a pre-built wheel from the official LIEF project, adapted for:

· ARM architecture (aarch64/armv7)
· Python 3.13 compatibility
· Mobile environment optimizations

⚡ Installation

```bash
pip install https://github.com/Gisnsl/lief-Termux/releases/download/1.0.0-00341b04/lief-1.0.0.dev0-py3-none-any.whl
```

✅ Requirements

· Python 3.13
· Termux or Pydroid3
· Internet connection (for download)

🚀 Quick Example

```python
import lief

# Parse a binary file
binary = lief.parse("/system/bin/ls")

# Print entry point
print(f"Entry point: 0x{binary.entrypoint:x}")

# List sections
for section in binary.sections:
    print(f"{section.name}: {section.size} bytes")
```

📱 Tested On

· ✅ Termux (Android 10+)
· ✅ Pydroid3 (v6.0+)
· ✅ Python 3.13

📚 Documentation

Full LIEF documentation: lief-project.github.io

🙏 Credits

· Original LIEF project by Romain Thomas
· Mobile adaptation by @maho_s9

📞 Support

Telegram: @maho_s9
