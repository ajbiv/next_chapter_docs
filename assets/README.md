# Assets

This folder contains images, diagrams, documents, and other media files referenced in the documentation.

## Folder Structure

```
assets/
├── images/                  # Screenshots, photos, icons
│   ├── screenshots/         # UI screenshots, demos
│   ├── logos/              # Brand assets, logos
│   ├── marketing/          # Marketing materials, social media
│   └── product/            # Product images, features
├── diagrams/               # Flowcharts, architecture diagrams, wireframes
│   ├── business/           # Business model, strategy diagrams
│   ├── technical/          # System architecture, technical flows
│   ├── process/            # Workflow diagrams, process maps
│   └── mindmaps/           # Brainstorming, concept maps
├── documents/              # PDFs, spreadsheets, external documents
│   ├── legal/              # Contracts, agreements, compliance
│   ├── financial/          # Financial statements, projections
│   ├── research/           # Market research, studies
│   └── presentations/      # Pitch decks, presentations
├── templates/              # Document templates, forms
│   ├── contracts/          # Legal document templates
│   ├── presentations/      # Slide templates
│   └── forms/              # Application forms, surveys
└── exports/                # Exported files from other tools
    ├── analytics/          # Data exports, reports
    ├── crm/               # Customer data exports
    └── tools/             # Exports from various business tools
```

## File Organization

### Images
- Use descriptive filenames
- Include date if relevant: `YYYY-MM-DD-description.png`
- Optimize file sizes for web viewing
- Supported formats: PNG, JPG, SVG, WebP

### Diagrams
- Save source files when possible (e.g., .drawio, .miro)
- Export to PNG/SVG for embedding in markdown
- Use consistent naming: `diagram-type-description.png`

### Documents
- Include version numbers when relevant
- Use clear, descriptive names
- Maintain original format when possible

## Linking Assets

Reference assets in markdown using relative paths:
```markdown
![Description](../assets/images/screenshot.png)
[Document Name](../assets/documents/specification.pdf)
```

## Asset Management Best Practices

### File Organization
- Keep file sizes reasonable (< 5MB for images, < 10MB for documents)
- Use version control friendly formats when possible
- Organize by project or topic when folders grow large
- Clean up unused assets periodically
- Use consistent naming: `YYYY-MM-DD-description-v1.0.ext`

### Version Control
- Include version numbers for important assets: `logo-v2.1.png`
- Keep source files when possible (e.g., `.sketch`, `.figma`, `.psd`)
- Document asset creation tools and requirements
- Use Git LFS for large binary files

### Screenshot Management
- Use consistent screenshot standards (resolution, browser, etc.)
- Include date and context in filenames
- Crop and optimize for web viewing
- Store both full and cropped versions when needed

### Diagram Creation Tools
- **Mermaid**: For simple diagrams embedded in markdown
- **Draw.io/Diagrams.net**: For complex business diagrams
- **Excalidraw**: For hand-drawn style diagrams
- **Figma/Sketch**: For UI/UX wireframes and mockups
- **Lucidchart**: For professional flowcharts and org charts

### Brand Asset Guidelines
- Maintain consistent brand colors, fonts, and styles
- Store brand guidelines document
- Keep high-resolution versions for print
- Optimize web versions for digital use
