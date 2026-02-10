---
name: "drawio"
displayName: "Draw.io Diagrams"
description: "Create and edit draw.io diagram files (.drawio) for architecture diagrams, flowcharts, network diagrams ..."
keywords: ["drawio", "diagram", "architecture", "flowchart", "network", "topology", "wireframe", "visual", "draw.io", "diagrams.net"]
---

# Draw.io Diagram Power

Create professional, editable diagram files in draw.io's native XML format.

## Output Format

Draw.io files are XML with this structure:

```xml
<mxfile host="app.diagrams.net" modified="DATE" agent="Claude" version="21.0.0" type="device">
  <diagram name="DIAGRAM_NAME" id="UNIQUE_ID">
    <mxGraphModel dx="1200" dy="800" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="1100" pageHeight="850" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <!-- All diagram elements go here -->
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
```

## Core Element Types

### Basic Shapes

```xml
<!-- Rectangle -->
<mxCell id="unique-id" value="Label Text" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="120" height="60" as="geometry" />
</mxCell>

<!-- Rounded Rectangle -->
<mxCell id="unique-id" value="Label" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="120" height="60" as="geometry" />
</mxCell>

<!-- Cylinder (Database) -->
<mxCell id="unique-id" value="Database" style="shape=cylinder3;whiteSpace=wrap;html=1;boundedLbl=1;backgroundOutline=1;size=15;fillColor=#f8cecc;strokeColor=#b85450;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="80" height="80" as="geometry" />
</mxCell>

<!-- Ellipse -->
<mxCell id="unique-id" value="Node" style="ellipse;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="80" height="80" as="geometry" />
</mxCell>
```

### Containers & Groups

```xml
<!-- Swimlane (Container with Header) -->
<mxCell id="unique-id" value="Section Title" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=30;fillColor=#f5f5f5;strokeColor=#666666;fontColor=#333333;" vertex="1" parent="1">
  <mxGeometry x="40" y="40" width="200" height="150" as="geometry" />
</mxCell>

<!-- Header Bar (using brand primary color) -->
<mxCell id="unique-id" value="" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#0066CC;strokeColor=#0066CC;" vertex="1" parent="1">
  <mxGeometry x="40" y="40" width="400" height="40" as="geometry" />
</mxCell>
```

### Connectors & Arrows

```xml
<!-- Basic Arrow -->
<mxCell id="unique-id" value="" style="endArrow=classic;html=1;rounded=0;strokeWidth=2;strokeColor=#666666;" edge="1" parent="1" source="source-id" target="target-id">
  <mxGeometry relative="1" as="geometry" />
</mxCell>

<!-- Bidirectional Arrow -->
<mxCell id="unique-id" value="" style="endArrow=classic;startArrow=classic;html=1;rounded=0;strokeWidth=2;" edge="1" parent="1">
  <mxGeometry relative="1" as="geometry">
    <mxPoint x="200" y="200" as="sourcePoint" />
    <mxPoint x="400" y="200" as="targetPoint" />
  </mxGeometry>
</mxCell>

<!-- Flex Arrow (Block Arrow) -->
<mxCell id="unique-id" value="" style="shape=flexArrow;endArrow=classic;html=1;fillColor=#FFB800;strokeColor=#cc9400;width=20;endSize=8;" edge="1" parent="1">
  <mxGeometry relative="1" as="geometry">
    <mxPoint x="200" y="200" as="sourcePoint" />
    <mxPoint x="400" y="200" as="targetPoint" />
  </mxGeometry>
</mxCell>

<!-- Dashed Line -->
<mxCell id="unique-id" value="" style="endArrow=classic;html=1;dashed=1;dashPattern=8 8;strokeColor=#999999;" edge="1" parent="1">
  <mxGeometry relative="1" as="geometry">
    <mxPoint x="200" y="200" as="sourcePoint" />
    <mxPoint x="400" y="200" as="targetPoint" />
  </mxGeometry>
</mxCell>
```

### Text Elements

```xml
<!-- Plain Text -->
<mxCell id="unique-id" value="Label Text" style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;fontSize=12;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="100" height="30" as="geometry" />
</mxCell>

<!-- Bold Title -->
<mxCell id="unique-id" value="Title" style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;fontSize=18;fontStyle=1;fontColor=#333333;" vertex="1" parent="1">
  <mxGeometry x="100" y="20" width="300" height="40" as="geometry" />
</mxCell>

<!-- Multi-line Text (use &#xa; for newlines) -->
<mxCell id="unique-id" value="Line 1&#xa;Line 2&#xa;Line 3" style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=top;whiteSpace=wrap;rounded=0;fontSize=10;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="150" height="60" as="geometry" />
</mxCell>
```

## Common Style Properties

### Colors (use hex codes)

| Property | Purpose | Example |
|----------|---------|---------|
| `fillColor` | Background | `fillColor=#dae8fc` |
| `strokeColor` | Border | `strokeColor=#6c8ebf` |
| `fontColor` | Text | `fontColor=#333333` |

### Standard Color Palette

```
Blue:    fillColor=#dae8fc;strokeColor=#6c8ebf
Green:   fillColor=#d5e8d4;strokeColor=#82b366
Yellow:  fillColor=#fff2cc;strokeColor=#d6b656
Orange:  fillColor=#ffe6cc;strokeColor=#d79b00
Red:     fillColor=#f8cecc;strokeColor=#b85450
Purple:  fillColor=#e1d5e7;strokeColor=#9673a6
Grey:    fillColor=#f5f5f5;strokeColor=#666666
```

### Typography

| Property | Values | Example |
|----------|--------|---------|
| `fontSize` | Number | `fontSize=12` |
| `fontStyle` | 0=normal, 1=bold, 2=italic, 3=bold+italic | `fontStyle=1` |
| `align` | left, center, right | `align=center` |
| `verticalAlign` | top, middle, bottom | `verticalAlign=middle` |

### Borders & Effects

| Property | Values | Example |
|----------|--------|---------|
| `rounded` | 0 or 1 | `rounded=1` |
| `strokeWidth` | Number | `strokeWidth=2` |
| `dashed` | 0 or 1 | `dashed=1` |
| `dashPattern` | Pattern | `dashPattern=8 8` |
| `shadow` | 0 or 1 | `shadow=1` |

## Company Branding (Customisable)

This power supports company-specific branding. Edit `steering/branding.md` to set your organisation's colours and styles.

**Default brand placeholders (replace with your own):**
```
Primary:   fillColor=#0066CC;strokeColor=#0052a3;fontColor=#FFFFFF
Secondary: fillColor=#FFB800;strokeColor=#cc9400;fontColor=#333333
Dark:      fillColor=#1a1a2e;strokeColor=#1a1a2e;fontColor=#FFFFFF
Light BG:  fillColor=#f0f4f8;strokeColor=#0066CC
```

See `steering/branding.md` for full customisation instructions.

## Diagram Patterns

### Architecture Diagram Layout

1. **Title bar** at top (full width, branded color)
2. **Main sections** as swimlanes or rounded containers
3. **Components** as rounded rectangles inside sections
4. **Databases** as cylinders
5. **External systems** on left/right edges
6. **Arrows** showing data/control flow
7. **Legend** in corner explaining colors/symbols
8. **Footer** with metadata

### Layered Architecture (Top to Bottom)

```
+-----------------------------------------+
|           Users / Clients               |  <- Top layer
+-----------------------------------------+
|           API / Interface               |
+-----------------------------------------+
|         Business Logic                  |
+-----------------------------------------+
|         Data / Storage                  |  <- Bottom layer
+-----------------------------------------+
```

### Left-to-Right Flow

```
+--------+     +----------+     +----------+
| Source  | --> | Process  | --> |  Target  |
+--------+     +----------+     +----------+
```

## Best Practices

1. **Unique IDs**: Every mxCell needs a unique `id` attribute
2. **Parent hierarchy**: Set `parent="1"` for top-level elements
3. **Positioning**: Use `mxGeometry` with x, y, width, height
4. **Layering**: Elements defined later appear on top
5. **Alignment**: Use consistent x/y spacing (grid of 10-20px)
6. **Colors**: Use coordinated fill/stroke pairs from the palette
7. **Labels**: Keep text concise; use separate text elements for descriptions
8. **Whitespace**: Leave margins inside containers (20-40px padding)

## Workflow

1. Determine diagram type and layout pattern
2. Set page dimensions in `mxGraphModel` (pageWidth, pageHeight)
3. Create container structure (swimlanes, groups)
4. Add components with unique IDs
5. Add connectors referencing source/target IDs
6. Add labels and annotations
7. Add legend if using color coding
8. Save as `.drawio` file

## Cloud Provider Icons (AWS, Azure, GCP)

Draw.io includes built-in shape libraries for major cloud providers. Use official icons for professional architecture diagrams.

### AWS Icons (Quick Reference)

AWS uses `shape=mxgraph.aws4.resourceIcon` with `resIcon=mxgraph.aws4.SERVICE`:

```xml
<mxCell id="lambda-1" value="Lambda" style="sketch=0;outlineConnect=0;fontColor=#232F3E;fillColor=#ED7100;strokeColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.lambda;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="78" height="78" as="geometry" />
</mxCell>
```

**Common AWS resIcon values:**
- Compute: `ec2`, `lambda`, `ecs`, `eks`, `fargate`
- Storage: `s3`, `elastic_block_store`, `elastic_file_system`
- Database: `rds`, `dynamodb`, `aurora`, `elasticache`, `redshift`
- Networking: `vpc`, `cloudfront`, `route_53`, `api_gateway`, `elastic_load_balancing`
- Security: `iam`, `cognito`, `secrets_manager`, `kms`, `waf`

**AWS Category Colors:**
- Compute: `#ED7100`
- Storage: `#7AA116`
- Database: `#C925D1`
- Networking: `#8C4FFF`
- Security: `#DD344C`

### Azure Icons (Quick Reference)

Azure uses `image=img/lib/azure2/CATEGORY/SERVICE.svg`:

```xml
<mxCell id="vm-1" value="VM" style="aspect=fixed;html=1;points=[];align=center;image;fontSize=12;image=img/lib/azure2/compute/Virtual_Machine.svg;verticalLabelPosition=bottom;verticalAlign=top;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="68" height="68" as="geometry" />
</mxCell>
```

**Common Azure image paths:**
- `compute/Virtual_Machine.svg`, `compute/Function_Apps.svg`
- `containers/Kubernetes_Services.svg`
- `storage/Storage_Accounts.svg`, `storage/Blob_Storage.svg`
- `databases/SQL_Database.svg`, `databases/Azure_Cosmos_DB.svg`
- `networking/Virtual_Networks.svg`, `networking/Load_Balancers.svg`
- `security/Key_Vaults.svg`, `identity/Azure_Active_Directory.svg`

### AWS Group Containers

```xml
<!-- VPC -->
<mxCell id="vpc" value="VPC" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_vpc;strokeColor=#8C4FFF;fillColor=none;verticalAlign=top;align=left;spacingLeft=30;dashed=0;" vertex="1" parent="1">
  <mxGeometry x="40" y="40" width="400" height="300" as="geometry" />
</mxCell>

<!-- Public Subnet -->
grIcon=mxgraph.aws4.group_public_subnet;strokeColor=#7AA116;fillColor=#E9F3E6

<!-- Private Subnet -->
grIcon=mxgraph.aws4.group_private_subnet;strokeColor=#00A4A6;fillColor=#E6F6F7
```

## References

For advanced patterns and complete icon lists, see:
- `steering/architecture-patterns.md` - Common architecture diagram layouts
- `steering/style-guide.md` - Extended styling options and icon placement
- `steering/cloud-icons.md` - Complete AWS, Azure, GCP icon reference
- `steering/branding.md` - Company branding customisation guide
