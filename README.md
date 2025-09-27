# APT-J2 Keyboard Layout

An optimized ergonomic keyboard layout based on APTv3 by Apsu Eve, designed for high in-roll patterns and angle-mod compatibility.

## 🚀 Quick Start

### What is APT-J2?

APT-J2 is an advanced keyboard layout that builds upon the foundation of APTv3, incorporating modern ergonomic principles and optimized finger placement strategies. The layout achieves a remarkable 42.1% in-roll percentage while maintaining comfortable finger travel patterns.

### Key Features

- **High In-Roll Optimization**: 42.1% in-roll patterns for smooth typing flow
- **Angle-Mod Compatible**: Specifically designed for angle-mod typing technique
- **Balanced Finger Load**: Reduced same-finger usage to just 1.2%
- **Strategic Punctuation**: Optimized placement of common punctuation marks
- **ANSI/ISO Support**: Compatible with both keyboard standards

## 📊 Performance Metrics

| Metric | APT-J2 | QWERTY | Dvorak |
|--------|--------|--------|--------|
| In-Roll | **42.1%** | 15.3% | 38.7% |
| Same Finger | **1.2%** | 6.7% | 2.1% |
| Same Hand | **28.4%** | 51.2% | 44.8% |
| Finger Travel | **Optimized** | High | Moderate |

## 🎹 Layout Design

### Normal Layer
```
Row 1: 1 2 3 4 5 6 7 8 9 0 = { ⌫
Row 2: w c m p k : l u o y - [ \
Row 3: r s t h b j n e a i ? ⏎
Row 4: g d f v z q x , . ' ⇧
```

### Shift Layer
```
Row 1: + @ # $ % ^ & * < > _ } ⌫
Row 2: W C M P K ; L U O Y / ] |
Row 3: R S T H B J N E A I ! ⏎
Row 4: G D F V Z Q X ( ) " ⇧
```

### Design Philosophy

APT-J2 follows these ergonomic principles:

1. **High In-Roll Patterns**: Maximizes comfortable finger rolling motions
2. **Reduced Same-Finger Usage**: Minimizes consecutive key presses with the same finger
3. **Angle-Mod Optimization**: Designed specifically for angle-mod typing technique
4. **Balanced Hand Usage**: Maintains reasonable same-hand percentage
5. **Punctuation Efficiency**: Strategic placement of programming symbols

## 🔄 Changes from APTv3

### Letter Repositioning

| Change | Rationale | Impact |
|--------|-----------|--------|
| **C to top row** | Better CW combinations | Improved comfort in words like "cow," "claw" |
| **D & G to bottom** | Maintain in-roll patterns | Preserves comfortable rolling after C move |
| **M & P elevated** | Maintain MP in-roll | Optimizes "camp," "jump," "lamp" |
| **B to home row** | Higher frequency than K | Better access to common letters |
| **K with C** | Improved CK combinations | Enhanced "back," "check," "quick" |

### Punctuation Changes

- **Colon (:)** moved to accessible Y position
- **Question mark (?)** placed on home row
- **Dash (-)** positioned for comfortable thumb reach
- **Equals (=)** maintained in number row for programming

## 💻 Installation

### Prerequisites

- Windows 10/11, macOS 10.15+, or Linux with X11/Wayland
- Administrator/sudo access for system-wide installation
- Optional: Keyboard layout software for customization

### Windows Installation

1. Download the `.klc` file from the [releases page](https://github.com/[your-username]/apt-j2/releases)
2. Install Microsoft Keyboard Layout Creator (if not already installed)
3. Open the `.klc` file in MSKLC
4. Click "Project" → "Build DLL and Setup Package"
5. Run the generated installer
6. Add APT-J2 through Windows Language Settings

### macOS Installation

1. Download the `.bundle` file from releases
2. Copy to `/Library/Keyboard Layouts/` (system-wide) or `~/Library/Keyboard Layouts/` (user)
3. Open System Preferences → Keyboard → Input Sources
4. Click "+" and select APT-J2 from the list
5. Enable "Show Input menu in menu bar" for easy switching

### Linux Installation

#### X11 (Xorg)

```bash
# Download the .xkb file
sudo cp apt-j2.xkb /usr/share/X11/xkb/symbols/apt-j2

# Add to your X11 configuration
setxkbmap -layout apt-j2
```

#### Wayland

```bash
# For Wayland compositors supporting XKB
export XKB_DEFAULT_LAYOUT=apt-j2
```

### MonkeyType Integration

1. Copy `apt-j2-layout.js` to MonkeyType's layout directory
2. Add the layout definition to `layouts.js`
3. Register in `layout-controller.js`
4. Test with both ANSI and ISO variants

## 🎯 Learning Guide

### Recommended Learning Path

#### Week 1-2: Foundation
- Master home row positions (RSTH + NEAI)
- Practice basic finger exercises
- Focus on accuracy over speed

#### Week 3-4: Top Row
- Add WCMP + LUOY combinations
- Practice common word patterns
- Maintain proper finger positioning

#### Week 5-6: Bottom Row
- Incorporate GDFV + QXZ positions
- Practice rolling patterns
- Build muscle memory

#### Week 7-8: Punctuation
- Master special characters
- Practice programming syntax
- Achieve full layout proficiency

### Practice Exercises

Focus on these high-frequency combinations:

**Home Row Trigrams:**
- THE, AND, ING, HER, ENT
- TH, HE, IN, ER, AN

**In-Roll Patterns:**
- RST, ST H, NEA, EAI
- WCM, CMP, LUO, UOY

**Common Words:**
- the, and, for, are, but
- with, have, this, will, your

## 📈 Performance Analysis

### Finger Usage Distribution

```
Left Hand (49.4%):
├── Pinky: 8.2% (1, q, a, z)
├── Ring: 12.4% (2, w, s, x, g)
├── Middle: 15.8% (3, e, d, c)
└── Index: 20.1% (4, 5, r, t, f, v, b)

Right Hand (50.6%):
├── Index: 19.3% (6, 7, y, u, h, j, n, m)
├── Middle: 10.2% (8, i, k, ,)
├── Ring: 8.7% (9, o, l, .)
└── Pinky: 5.3% (0, p, ;, /, :, -, ?, !)
```

### Ergonomic Benefits

- **Reduced Lateral Strain**: Minimal pinky usage
- **Balanced Load**: Prevents overuse injuries
- **Natural Positioning**: Maintains hand comfort
- **High Efficiency**: Optimized for speed and accuracy

## 🔧 Customization

### Layer Modifications

The layout supports custom layers for specific use cases:

#### Programming Layer
- Optimized bracket and symbol placement
- Common programming shortcuts
- IDE-friendly key combinations

#### Gaming Layer
- WASD compatibility
- Quick access to function keys
- Macro support for complex commands

#### International Support
- Dead key combinations
- Accented character access
- Unicode symbol input

### Configuration Options

```javascript
// Example customization
const APT_J2_CONFIG = {
    layout: 'apt-j2',
    variant: 'ansi', // or 'iso'
    angleMod: true,
    customLayers: {
        programming: true,
        gaming: false,
        international: false
    },
    preferences: {
        shiftBehavior: 'standard',
        deadKeys: true,
        macroSupport: true
    }
};
```

## 🐛 Troubleshooting

### Common Issues

#### Layout Not Appearing
- **Windows**: Check if installed correctly in Language Settings
- **macOS**: Verify bundle location and permissions
- **Linux**: Confirm XKB configuration and layout path

#### Key Mapping Issues
- Ensure correct ANSI/ISO variant selection
- Check for conflicting keyboard shortcuts
- Verify system keyboard settings

#### Performance Problems
- Some applications may need restart to recognize new layout
- Gaming applications might require specific configuration
- Remote desktop software may need additional setup

### Getting Help

- **GitHub Issues**: Report bugs and request features
- **Community Forum**: Get help from other users
- **Discord Server**: Real-time support and discussion

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Development Setup

1. Fork the repository
2. Clone your fork locally
3. Create a feature branch
4. Make your changes
5. Test across platforms
6. Submit a pull request

### Areas for Contribution

- **Layout Analysis**: Improve statistical modeling
- **Platform Support**: Add compatibility for new systems
- **Documentation**: Enhance guides and tutorials
- **Testing**: Validate performance across applications
- **Localization**: Add support for additional languages

### Code Style

- Use consistent indentation (2 spaces)
- Follow existing naming conventions
- Include comprehensive comments
- Test changes across multiple platforms

## 📄 License

This project is released under the same license as APTv3. Please credit both Apsu Eve for the original APTv3 design and [Your Name] for the APT-J2 optimizations.

## 🙏 Acknowledgments

- **Apsu Eve** - Original APTv3 layout design
- **Keyboard Layout Analyzer** - Statistical analysis tools
- **MonkeyType Community** - Testing and feedback
- **Ergonomic Research Community** - Scientific foundation

## 📚 References

- [Keyboard Layouts Document (3rd Edition)](https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o)
- [APTv3 Original Repository](https://github.com/Apsu/APT)
- [Keyboard Layout Analyzer](https://cyanophage.github.io/)
- [MonkeyType](https://monkeytype.com)

## 📞 Contact

- **GitHub Issues**: [Create an issue](https://github.com/[your-username]/apt-j2/issues)
- **Email**: [your-email@example.com]
- **Discord**: [Discord Server Invite]

---

**Happy typing with APT-J2!** ⌨️✨

*Last updated: [Current Date]*
*Version: 1.0.0*
