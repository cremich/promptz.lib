# Company Branding Configuration

This file defines organisation-specific colours and styles for diagrams. Customise these values to match your company's brand guidelines.

## How to Customise

1. Replace the placeholder hex codes with your company colours
2. Update the example company name references
3. Adjust the accent colours to complement your primary brand

---

## Brand Color Definitions

### Primary Brand Colors

Replace these with your organisation's colours:

```
# Primary (main brand color - headers, key elements)
Primary:      fillColor=#0066CC;strokeColor=#0052a3;fontColor=#FFFFFF

# Secondary (accent color - highlights, call-to-action elements)
Secondary:    fillColor=#FFB800;strokeColor=#cc9400;fontColor=#333333

# Dark (footers, dark backgrounds)
Dark:         fillColor=#1a1a2e;strokeColor=#1a1a2e;fontColor=#FFFFFF

# Light Background (containers, zones)
Light BG:     fillColor=#f0f4f8;strokeColor=#0066CC
```

### Calculating Stroke Colors

For professional results, stroke colors should be ~20% darker than fill colors:

| Fill Color | Stroke Calculation | Result |
|------------|-------------------|--------|
| `#0066CC` | Reduce each RGB by 20% | `#0052a3` |
| `#FFB800` | Reduce each RGB by 20% | `#cc9400` |

**Quick method:** Use an online color darkener or multiply each RGB value by 0.8.

---

## Standard Brand Applications

### Header Bar (Top of Diagrams)

```xml
<!-- Branded header bar -->
<mxCell id="header" value="" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#0066CC;strokeColor=#0066CC;" vertex="1" parent="1">
  <mxGeometry x="40" y="40" width="1020" height="40" as="geometry" />
</mxCell>

<!-- Company name in header -->
<mxCell id="header-title" value="Your Company Name" style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;whiteSpace=wrap;rounded=0;fontSize=14;fontStyle=1;fontColor=#FFFFFF;" vertex="1" parent="1">
  <mxGeometry x="50" y="45" width="200" height="30" as="geometry" />
</mxCell>
```

### Platform/Service Zone (Center Focus Area)

```xml
<!-- Branded central zone -->
<mxCell id="platform-zone" value="" style="rounded=1;fillColor=#0066CC;strokeColor=#0066CC;opacity=90;" vertex="1" parent="1">
  <mxGeometry x="380" y="100" width="300" height="400" as="geometry" />
</mxCell>

<!-- Zone title (white text on brand color) -->
<mxCell id="zone-title" value="Your Platform" style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;fontStyle=1;fontSize=14;fontColor=#FFFFFF;" vertex="1" parent="1">
  <mxGeometry x="380" y="110" width="300" height="30" as="geometry" />
</mxCell>
```

### Accent Arrows (Data Flow, Replication)

```xml
<!-- Branded flex arrow -->
<mxCell id="flow-arrow" value="" style="shape=flexArrow;endArrow=classic;html=1;fillColor=#FFB800;strokeColor=#cc9400;width=20;endSize=8;" edge="1" parent="1">
  <mxGeometry relative="1" as="geometry">
    <mxPoint x="200" y="200" as="sourcePoint" />
    <mxPoint x="400" y="200" as="targetPoint" />
  </mxGeometry>
</mxCell>
```

### Footer Bar

```xml
<!-- Dark footer bar -->
<mxCell id="footer" value="" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#1a1a2e;strokeColor=#1a1a2e;" vertex="1" parent="1">
  <mxGeometry x="40" y="760" width="1020" height="30" as="geometry" />
</mxCell>

<!-- Footer text -->
<mxCell id="footer-text" value="© Your Company | Architecture Diagram | Last Updated: DATE" style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;fontSize=9;fontColor=#FFFFFF;" vertex="1" parent="1">
  <mxGeometry x="40" y="760" width="1020" height="30" as="geometry" />
</mxCell>
```

---

## Example Brand Configurations

### Tech Company (Blue/Orange)

```
Primary:    fillColor=#0066CC;strokeColor=#0052a3;fontColor=#FFFFFF
Secondary:  fillColor=#FF6B00;strokeColor=#cc5500;fontColor=#FFFFFF
Dark:       fillColor=#1a1a2e;strokeColor=#1a1a2e;fontColor=#FFFFFF
Light BG:   fillColor=#e8f4fc;strokeColor=#0066CC
```

### Healthcare (Teal/Green)

```
Primary:    fillColor=#008B8B;strokeColor=#006f6f;fontColor=#FFFFFF
Secondary:  fillColor=#90EE90;strokeColor=#73be73;fontColor=#333333
Dark:       fillColor=#2F4F4F;strokeColor=#2F4F4F;fontColor=#FFFFFF
Light BG:   fillColor=#E0FFFF;strokeColor=#008B8B
```

### Finance (Navy/Gold)

```
Primary:    fillColor=#1B365D;strokeColor=#162b4a;fontColor=#FFFFFF
Secondary:  fillColor=#C5A572;strokeColor=#9e845b;fontColor=#333333
Dark:       fillColor=#0D1B2A;strokeColor=#0D1B2A;fontColor=#FFFFFF
Light BG:   fillColor=#F5F5F0;strokeColor=#1B365D
```

### Government/Public Sector (Dark Blue/Red)

```
Primary:    fillColor=#003366;strokeColor=#002952;fontColor=#FFFFFF
Secondary:  fillColor=#CC0000;strokeColor=#a30000;fontColor=#FFFFFF
Dark:       fillColor=#1C1C1C;strokeColor=#1C1C1C;fontColor=#FFFFFF
Light BG:   fillColor=#F0F0F0;strokeColor=#003366
```

---

## Color Accessibility Notes

When choosing brand colors for diagrams:

1. **Contrast ratio**: Ensure text has sufficient contrast against backgrounds (WCAG AA minimum 4.5:1)
2. **Color blindness**: Don't rely solely on color to convey meaning—use patterns, labels, or icons
3. **Print-friendly**: Test how diagrams look in grayscale for printing
4. **Consistent meaning**: Use the same colors for the same concepts across all diagrams

---

## Quick Reference: Style Strings

Copy-paste ready style snippets:

```
# Header bar
fillColor=#0066CC;strokeColor=#0066CC

# Central branded zone
fillColor=#0066CC;strokeColor=#0066CC;rounded=1;opacity=90

# Accent arrow
fillColor=#FFB800;strokeColor=#cc9400

# Footer bar
fillColor=#1a1a2e;strokeColor=#1a1a2e

# Light container background
fillColor=#f0f4f8;strokeColor=#0066CC;rounded=1

# White text on brand
fontColor=#FFFFFF;fontSize=14;fontStyle=1

# Dark text on light
fontColor=#333333;fontSize=12
```
