# Draw.io Style Guide

Extended styling options, icon placeholders, and patterns.

## Table of Contents

1. [Icon Placeholders](#icon-placeholders)
2. [Advanced Shapes](#advanced-shapes)
3. [Shadow and Effects](#shadow-and-effects)
4. [Arrow Styles](#arrow-styles)
5. [Status Indicators](#status-indicators)

---

## Icon Placeholders

Use emoji or text placeholders that users can replace with actual service icons:

### Compute & Servers

```xml
<!-- Server with emoji placeholder -->
<mxCell id="server" value="🖥️" style="text;fontSize=24;align=center;verticalAlign=middle;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="40" height="40" as="geometry" />
</mxCell>

<!-- VM Icon placeholder -->
<mxCell id="vm" value="[VM]" style="rounded=1;fillColor=#dae8fc;strokeColor=#6c8ebf;fontStyle=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="60" height="40" as="geometry" />
</mxCell>
```

### Common Emoji Placeholders

| Service Type | Emoji | Alternative |
|--------------|-------|-------------|
| Server/VM | 🖥️ | [VM] |
| Database | 🗄️ | [DB] |
| Storage | 💾 | [DISK] |
| Network | 🌐 | [NET] |
| Security | 🔒 | [SEC] |
| User | 👤 | [USER] |
| Users | 👥 | [USERS] |
| Cloud | ☁️ | [CLOUD] |
| Container | 📦 | [CTR] |
| API | 🔌 | [API] |
| Queue | 📬 | [MQ] |
| Monitor | 📊 | [MON] |
| Settings | ⚙️ | [CFG] |
| Sync | 🔄 | [SYNC] |
| Warning | ⚠️ | [WARN] |
| Success | ✅ | [OK] |
| Time/Schedule | ⏱️ | [TIME] |
| Lightning/Fast | ⚡ | [FAST] |

### Placeholder Box Pattern

Create a box that users can drop icons into:

```xml
<!-- Icon placeholder box -->
<mxCell id="icon-placeholder" value="" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#FFFFFF;strokeColor=#999999;strokeWidth=1;dashed=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="60" height="60" as="geometry" />
</mxCell>
<mxCell id="icon-hint" value="[Icon]" style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;fontSize=9;fontColor=#999999;" vertex="1" parent="1">
  <mxGeometry x="100" y="120" width="60" height="20" as="geometry" />
</mxCell>
```

---

## Advanced Shapes

### Cloud Shape

```xml
<mxCell id="cloud" value="Cloud" style="ellipse;shape=cloud;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="120" height="80" as="geometry" />
</mxCell>
```

### Document Shape

```xml
<mxCell id="doc" value="Doc" style="shape=document;whiteSpace=wrap;html=1;boundedLbl=1;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="80" height="60" as="geometry" />
</mxCell>
```

### Hexagon

```xml
<mxCell id="hex" value="Service" style="shape=hexagon;perimeter=hexagonPerimeter2;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="100" height="80" as="geometry" />
</mxCell>
```

### Parallelogram (Data/Input)

```xml
<mxCell id="data" value="Data" style="shape=parallelogram;perimeter=parallelogramPerimeter;whiteSpace=wrap;html=1;fillColor=#ffe6cc;strokeColor=#d79b00;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="100" height="50" as="geometry" />
</mxCell>
```

### Diamond (Decision)

```xml
<mxCell id="decision" value="?" style="rhombus;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="80" height="80" as="geometry" />
</mxCell>
```

### Callout

```xml
<mxCell id="callout" value="Note text" style="shape=callout;whiteSpace=wrap;html=1;perimeter=calloutPerimeter;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="120" height="80" as="geometry" />
</mxCell>
```

---

## Shadow and Effects

### Drop Shadow

```xml
style="...;shadow=1;"
```

### Gradient Fill

```xml
style="...;fillColor=#dae8fc;gradientColor=#ffffff;gradientDirection=south;"
```

### Opacity

```xml
style="...;opacity=70;"
```

### Glass Effect

```xml
style="...;glass=1;"
```

---

## Arrow Styles

### Arrow End Styles

| Style | Property |
|-------|----------|
| Classic arrow | `endArrow=classic` |
| Open arrow | `endArrow=open` |
| Block arrow | `endArrow=block` |
| Diamond | `endArrow=diamond` |
| Circle | `endArrow=oval` |
| None | `endArrow=none` |

### Line Styles

```xml
<!-- Solid -->
style="strokeWidth=2;"

<!-- Dashed -->
style="dashed=1;dashPattern=8 8;"

<!-- Dotted -->
style="dashed=1;dashPattern=2 2;"

<!-- Thick -->
style="strokeWidth=4;"
```

### Orthogonal Routing (Right Angles)

```xml
<mxCell id="edge" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;" edge="1" parent="1">
```

### Curved Routing

```xml
<mxCell id="edge" style="edgeStyle=elbowEdgeStyle;elbow=vertical;rounded=1;" edge="1" parent="1">
```

---

## Status Indicators

### Traffic Light Pattern

```xml
<!-- Green (Active/Success) -->
<mxCell id="status-green" value="" style="ellipse;fillColor=#00CC00;strokeColor=#009900;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="15" height="15" as="geometry" />
</mxCell>

<!-- Yellow (Warning/Pending) -->
<mxCell id="status-yellow" value="" style="ellipse;fillColor=#FFCC00;strokeColor=#cc9900;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="15" height="15" as="geometry" />
</mxCell>

<!-- Red (Error/Down) -->
<mxCell id="status-red" value="" style="ellipse;fillColor=#FF0000;strokeColor=#cc0000;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="15" height="15" as="geometry" />
</mxCell>

<!-- Grey (Standby/Inactive) -->
<mxCell id="status-grey" value="" style="ellipse;fillColor=#CCCCCC;strokeColor=#999999;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="15" height="15" as="geometry" />
</mxCell>
```

### Badge Pattern

```xml
<mxCell id="badge" value="DR Ready" style="rounded=1;fillColor=#d5e8d4;strokeColor=#82b366;fontSize=10;fontStyle=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="70" height="24" as="geometry" />
</mxCell>
```

---

## Legend Template

```xml
<!-- Legend Container -->
<mxCell id="legend" value="" style="rounded=0;fillColor=#f5f5f5;strokeColor=#666666;" vertex="1" parent="1">
  <mxGeometry x="900" y="100" width="180" height="200" as="geometry" />
</mxCell>

<mxCell id="legend-title" value="Legend" style="text;fontSize=12;fontStyle=1;align=center;" vertex="1" parent="1">
  <mxGeometry x="900" y="105" width="180" height="20" as="geometry" />
</mxCell>

<!-- Legend Item -->
<mxCell id="legend-item-1" value="" style="rounded=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
  <mxGeometry x="915" y="135" width="20" height="15" as="geometry" />
</mxCell>
<mxCell id="legend-label-1" value="Source System" style="text;fontSize=9;align=left;" vertex="1" parent="1">
  <mxGeometry x="945" y="133" width="120" height="20" as="geometry" />
</mxCell>
```

---

## Page Size Presets

| Format | pageWidth | pageHeight |
|--------|-----------|------------|
| A4 Landscape | 1169 | 827 |
| A4 Portrait | 827 | 1169 |
| A3 Landscape | 1654 | 1169 |
| Letter Landscape | 1100 | 850 |
| Widescreen 16:9 | 1920 | 1080 |
| Slide 4:3 | 1024 | 768 |

Set in `<mxGraphModel>`:
```xml
<mxGraphModel ... pageWidth="1400" pageHeight="900" ...>
```
