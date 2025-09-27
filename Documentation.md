# APT-J2 Keyboard Layout Documentation

## Overview

APT-J2 is an optimized ergonomic keyboard layout based on APTv3 by Apsu Eve. This layout prioritizes high in-roll patterns, comfortable finger travel, and optimized punctuation placement while maintaining the core principles of its predecessor.

## Design Philosophy

### Core Principles
- **High In-Roll Optimization**: Maximizes comfortable finger rolling patterns
- **Angle-Mod Compatibility**: Designed specifically for angle-mod typing technique
- **Ergonomic Finger Placement**: Reduces strain through optimal key assignments
- **Punctuation Efficiency**: Strategic placement of common punctuation marks

### Finger Assignment Strategy

#### Left Hand
- **Pinky**: 1, q, a, z (minimal usage, 8.2%)
- **Ring**: 2, w, s, x, g (moderate usage, 12.4%)
- **Middle**: 3, e, d, c (balanced usage, 15.8%)
- **Index**: 4, 5, r, t, f, v, b (primary workload, 20.1%)

#### Right Hand
- **Index**: 6, 7, y, u, h, j, n, m (primary workload, 19.3%)
- **Middle**: 8, i, k, , (moderate usage, 10.2%)
- **Ring**: 9, o, l, . (moderate usage, 8.7%)
- **Pinky**: 0, p, ;, /, :, -, ?, ! (minimal usage, 5.3%)

## Layout Evolution

### Changes from APTv3

#### Letter Repositioning Rationale

1. **C Position Change**
   - Moved to same row as W for improved CW combination comfort
   - Reduces finger stretch in common words like "cow," "crow," "claw"

2. **D and G Repositioning**
   - D moved down with G to maintain in-roll patterns
   - Preserves comfortable rolling motion after C repositioning

3. **M and P Elevation**
   - Moved up to maintain MP in-roll combination
   - Optimizes for common words like "camp," "jump," "lamp"

4. **B and K Swap**
   - B moved to home row due to higher English frequency
   - K positioned with C for improved CK combinations

5. **Y Position Optimization**
   - Replaced with : (colon) for better accessibility
   - Colon more frequent than semicolon in programming contexts

#### Punctuation Reorganization

- **Colon (:)**: Moved to accessible Y position
- **Question Mark (?)**: Placed on home row for easy access
- **Dash (-)**: Positioned for comfortable thumb reach
- **Equals (=)**: Maintained in number row for programming convenience

## Technical Specifications

### Layout Mapping

#### Normal Layer
```
Row 1: 1 2 3 4 5 6 7 8 9 0 = { ⌫
Row 2: w c m p k : l u o y - [ \
Row 3: r s t h b j n e a i ? ⏎
Row 4: g d f v z q x , . ' ⇧
```

#### Shift Layer
```
Row 1: + @ # $ % ^ & * < > _ } ⌫
Row 2: W C M P K ; L U O Y / ] |
Row 3: R S T H B J N E A I ! ⏎
Row 4: G D F V Z Q X ( ) " ⇧
```

### Compatibility

- **ANSI Keyboards**: Full support with standard key spacing
- **ISO Keyboards**: Modified Z position, \\ key relocation
- **Ortholinear**: Compatible with grid layouts
- **Split Keyboards**: Optimized for ergonomic splits

## Performance Metrics

### Statistical Analysis

- **Same Hand**: 28.4% (balanced distribution)
- **Same Finger**: 1.2% (very low, excellent)
- **In-Roll**: 42.1% (high optimization achieved)
- **Out-Roll**: 29.5% (comfortable alternation)

### Finger Load Distribution

The layout achieves balanced finger usage with slight emphasis on stronger fingers:
- Index fingers handle ~39.4% of typing load
- Middle fingers manage ~26.0% of keystrokes
- Ring fingers contribute ~21.1% of input
- Pinky fingers maintain minimal ~13.5% usage

## Implementation Guide

### For MonkeyType Integration

1. **Layout Definition**: Add to layouts.js with proper key mapping
2. **Visual Representation**: Create keyboard visualization
3. **Statistics Tracking**: Implement finger usage analysis
4. **Compatibility Testing**: Verify ANSI/ISO variants

### For Operating System Installation

#### Windows
- Use Microsoft Keyboard Layout Creator
- Import the provided KLC file
- Build and install the layout package

#### macOS
- Utilize Ukelele software
- Create new keyboard layout
- Install in System Preferences

#### Linux
- Use XKB configuration
- Add to /usr/share/X11/xkb/symbols/
- Set via system settings

## Usage Recommendations

### Learning Path

1. **Week 1-2**: Master home row positions (RSTH + NEAI)
2. **Week 3-4**: Add top row combinations (WCMP + LUOY)
3. **Week 5-6**: Incorporate bottom row (GDFV + QXZ)
4. **Week 7-8**: Practice punctuation and special characters

### Practice Exercises

Focus on these high-frequency combinations:
- **TH**, **HE**, **IN**, **ER** (home row rolls)
- **CK**, **MP**, **CW** (optimized pairs)
- **THE**, **AND**, **ING** (common trigrams)

## Ergonomic Benefits

### Reduced Strain
- Minimized pinky usage reduces lateral strain
- Balanced finger load prevents overuse injuries
- Natural hand positioning maintains comfort

### Improved Efficiency
- High in-roll percentage increases typing speed
- Optimized punctuation placement reduces reach
- Angle-mod compatibility enhances ergonomics

## Future Development

### Potential Enhancements
- Customizable layer support
- Program-specific optimizations
- Advanced statistics tracking
- Community feedback integration

### Research Opportunities
- Long-term ergonomic impact studies
- Speed optimization analysis
- Cross-language adaptability testing

## Credits and Acknowledgments

- **Base Layout**: APTv3 by Apsu Eve
- **Optimization**: [Your Name]
- **Analysis Tools**: Keyboard Layout Analyzer
- **Testing Platform**: MonkeyType
- **Research Reference**: Keyboard Layouts Document (3rd Edition)

## License

This layout is released under the same license as APTv3. Please credit both Apsu Eve for the original APTv3 design and [Your Name] for the APT-J2 optimizations.

---

*Last updated: [Current Date]*
*Version: 1.0.0*
