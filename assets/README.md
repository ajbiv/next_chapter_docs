# Assets

This folder contains images, diagrams, documents, and other media files referenced in the documentation.

## Folder Structure

```
assets/
├── images/                  # Screenshots, photos, icons
├── diagrams/               # Flowcharts, architecture diagrams, wireframes
├── documents/              # PDFs, spreadsheets, external documents
├── templates/              # Document templates, forms
└── exports/                # Exported files from other tools
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

## Best Practices

- Keep file sizes reasonable (< 5MB for images)
- Use version control friendly formats when possible
- Organize by project or topic when the folder grows large
- Clean up unused assets periodically
