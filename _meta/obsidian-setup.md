# Obsidian Setup Guide

This guide helps you set up Obsidian to work optimally with this documentation project.

## Initial Setup

### 1. Add to Vault
- Open Obsidian
- Choose "Open folder as vault"
- Select the `docs-project` folder
- Or add this folder to an existing vault

### 2. Recommended Settings

#### Core Settings
- **Files & Links**
  - New link format: `Shortest path when possible`
  - Use `[[Wikilinks]]`: Enabled
  - Automatically update internal links: Enabled

- **Editor**
  - Readable line length: Enabled
  - Strict line breaks: Disabled
  - Show frontmatter: Enabled

#### Appearance
- Theme: Choose based on preference
- Font size: Adjust for comfort
- Line numbers: Enabled (helpful for long documents)

### 3. Recommended Core Plugins

Enable these core plugins:
- **Templates**: For using document templates
- **Daily notes**: For tracking progress
- **Graph view**: For visualizing document connections
- **Outline**: For document navigation
- **Tag pane**: For tag-based organization
- **File explorer**: For folder navigation
- **Search**: For finding content across documents

### 4. Template Configuration

#### Templates Plugin Setup
1. Enable Templates plugin
2. Set template folder location: `05-templates`
3. Set date format: `YYYY-MM-DD`
4. Set time format: `HH:mm`

#### Using Templates
- Use `Ctrl/Cmd + P` → "Templates: Insert template"
- Or create hotkeys for frequently used templates

### 5. Recommended Community Plugins

Consider installing these community plugins:
- **Advanced Tables**: Better table editing
- **Calendar**: Visual calendar for daily notes
- **Kanban**: Project management boards
- **Mind Map**: Visual mind mapping
- **Excalidraw**: Drawing and diagramming

## Workflow Tips

### Document Creation
1. Use templates from `05-templates/`
2. Follow naming conventions in folder READMEs
3. Add appropriate tags
4. Link to related documents

### Navigation
- Use `Ctrl/Cmd + O` for quick switcher
- Use `Ctrl/Cmd + Shift + F` for global search
- Use graph view to explore connections
- Use tag pane to find tagged content

### Linking Strategy
- Link related concepts: `[[concept-name]]`
- Use descriptive link text: `[[document-name|Display Text]]`
- Create index pages for major topics
- Use tags for categorization: `#planning #strategy`

### Daily Workflow
1. Start with daily note or project dashboard
2. Create/update documents as needed
3. Link new content to existing documents
4. Review and organize weekly

## File Organization

### Naming Conventions
- Use lowercase with hyphens: `project-plan.md`
- Include dates when relevant: `2025-12-09-meeting-notes.md`
- Be descriptive but concise

### Folder Usage
- Keep active work in main folders (01-05)
- Move completed work to `06-archive/`
- Use `assets/` for all media files
- Keep project config in `_meta/`

## Backup & Sync

### Git Integration
- This project uses Git for version control
- Commit changes regularly
- Use descriptive commit messages
- Consider using Obsidian Git plugin for automation

### Obsidian Sync
- Obsidian Sync can be used alongside Git
- Configure to sync settings but not content (handled by Git)
- Useful for syncing across devices

## Troubleshooting

### Common Issues
- **Links not working**: Check file paths and naming
- **Templates not appearing**: Verify template folder setting
- **Slow performance**: Consider excluding large folders from indexing
- **Sync conflicts**: Use Git to resolve conflicts

### Performance Optimization
- Exclude unnecessary folders from indexing
- Limit graph view to current folder when needed
- Use search filters to narrow results
- Regular cleanup of unused files
