# Git Workflow for Documentation Project

## Overview
This documentation project uses Git for version control to track changes, maintain history, and enable collaboration. This document outlines the Git workflow and best practices.

## Repository Structure
```
docs-project/
├── .git/                    # Git repository data
├── .gitignore              # Files to ignore in version control
├── README.md               # Project overview
├── windsurf-rules.md       # AI assistant guidelines
├── 01-planning/            # Planning documents
├── 02-specifications/      # Technical specifications
├── 03-business/           # Business analysis
├── 04-meetings/           # Meeting notes and decisions
├── 05-templates/          # Document templates
├── 06-archive/            # Archived documents
├── assets/                # Media files and attachments
└── _meta/                 # Project metadata
```

## Branching Strategy

### Main Branch
- `main`: Production-ready documentation
- Always stable and deployable
- Protected branch (if using remote repository)

### Feature Branches
- `feature/topic-name`: For new documentation initiatives
- `update/document-name`: For significant document updates
- `template/template-name`: For new template development

### Example Branch Names
- `feature/api-documentation`
- `update/project-roadmap`
- `template/user-story-template`

## Commit Message Standards

### Format
```
type(scope): brief description

Detailed explanation if needed

- List specific changes
- Reference related documents
```

### Types
- `feat`: New document or major content addition
- `update`: Significant updates to existing content
- `fix`: Corrections or error fixes
- `docs`: Documentation about the documentation project itself
- `template`: New or updated templates
- `archive`: Moving documents to archive
- `refactor`: Reorganizing without content changes

### Examples
```
feat(planning): add Q1 2025 project roadmap

- Created comprehensive roadmap for Q1 initiatives
- Included timeline with Mermaid Gantt chart
- Added stakeholder assignments and milestones
- Links to related specification documents

update(specs): revise API specification v2.1

- Updated authentication section
- Added new endpoint documentation
- Fixed formatting issues in examples
- Added Mermaid sequence diagrams

template(meetings): enhance meeting notes template

- Added section for AI assistant participation
- Included Mermaid diagram placeholder
- Enhanced action item tracking format
- Added related documents section
```

## Workflow Steps

### 1. Starting New Work
```bash
# Ensure you're on main branch
git checkout main

# Pull latest changes (if using remote)
git pull origin main

# Create feature branch
git checkout -b feature/new-documentation

# Start working on documents
```

### 2. Making Changes
```bash
# Stage specific files
git add path/to/document.md

# Or stage all changes
git add .

# Commit with descriptive message
git commit -m "feat(planning): add project charter document"
```

### 3. Regular Commits
- Commit frequently (daily or after significant changes)
- Each commit should represent a logical unit of work
- Use descriptive commit messages following the standards

### 4. Completing Work
```bash
# Final commit
git add .
git commit -m "feat(planning): finalize project charter with stakeholder review"

# Switch back to main
git checkout main

# Merge feature branch
git merge feature/new-documentation

# Delete feature branch
git branch -d feature/new-documentation
```

## File Management

### What to Commit
- All Markdown documents (`.md` files)
- Essential Obsidian configuration files
- Asset files (images, diagrams) under reasonable size limits
- Template files
- Project metadata

### What NOT to Commit
- Personal Obsidian workspace files (covered by `.gitignore`)
- Temporary files and backups
- Large binary files (>5MB)
- OS-generated files (`.DS_Store`, `Thumbs.db`)

### Large Files
For files larger than 5MB:
- Consider using Git LFS (Large File Storage)
- Or store externally and link in documentation
- Compress images when possible

## Collaboration Workflow

### Working with Others
1. **Pull before starting**: Always get latest changes
2. **Communicate changes**: Use descriptive commit messages
3. **Resolve conflicts**: Merge conflicts in Markdown are usually straightforward
4. **Review changes**: Use `git diff` to review before committing

### Handling Conflicts
```bash
# If merge conflicts occur
git status                    # See conflicted files
# Edit files to resolve conflicts
git add resolved-file.md      # Mark as resolved
git commit                    # Complete the merge
```

## Remote Repository Setup

### GitHub/GitLab Setup
```bash
# Add remote repository
git remote add origin https://github.com/username/docs-project.git

# Push initial commit
git push -u origin main

# For subsequent pushes
git push origin main
```

### Syncing with Remote
```bash
# Fetch and merge changes
git pull origin main

# Push local changes
git push origin main
```

## Backup Strategy

### Local Backups
- Git itself provides backup through commit history
- Consider periodic exports of important documents
- Use `git bundle` for offline backups

### Remote Backups
- Push to remote repository regularly
- Consider multiple remotes for redundancy
- Use cloud storage for additional backup

## Maintenance Tasks

### Regular Cleanup
```bash
# View commit history
git log --oneline

# Clean up merged branches
git branch -d old-feature-branch

# Compress repository (occasionally)
git gc
```

### Archive Management
- Move completed projects to `06-archive/` folder
- Commit archive operations with clear messages
- Keep archive organized by date/project

## Integration with Obsidian

### Obsidian Git Plugin
Consider installing the Obsidian Git plugin for:
- Automatic commits on schedule
- Easy staging and committing from Obsidian
- Visual diff viewing
- Simplified Git operations

### Manual Git Workflow
If not using the plugin:
- Use terminal/command line for Git operations
- Commit changes after each work session
- Use descriptive commit messages
- Review changes before committing

## Troubleshooting

### Common Issues
- **Merge conflicts**: Usually in frontmatter or formatting
- **Large files**: Use `.gitignore` or Git LFS
- **Accidental commits**: Use `git reset` or `git revert`
- **Lost changes**: Check `git reflog` for recovery

### Recovery Commands
```bash
# Undo last commit (keep changes)
git reset --soft HEAD~1

# Undo last commit (discard changes)
git reset --hard HEAD~1

# View reflog for recovery
git reflog

# Recover from reflog
git checkout <commit-hash>
```

---

**Tags**: #meta #git #workflow #version-control #collaboration
**Created**: 2025-12-09
**Last Updated**: 2025-12-09
