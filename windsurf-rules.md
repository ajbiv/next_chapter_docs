# Windsurf Documentation Rules

This file contains rules and guidelines for AI assistants (like Windsurf/Cascade) when working on this documentation project. These rules ensure consistency, quality, and proper use of Obsidian features.

## Core Documentation Principles

### 1. Structure & Organization
- **ALWAYS** use the established folder structure (01-planning, 02-specifications, etc.)
- **ALWAYS** follow naming conventions: lowercase with hyphens, dates in YYYY-MM-DD format
- **ALWAYS** place files in the most appropriate folder based on content type
- **ALWAYS** create README.md files for new folders explaining their purpose

### 2. Markdown Standards
- Use consistent heading hierarchy (# for title, ## for main sections, ### for subsections)
- Use **bold** for emphasis, *italics* for subtle emphasis
- Use `code blocks` for technical terms, file names, and commands
- Use > blockquotes for important notes or warnings
- Always include a blank line before and after headings, lists, and code blocks

### 3. Obsidian Features Integration

#### Wikilinks
- **ALWAYS** use `[[wikilinks]]` to connect related documents
- Use descriptive link text: `[[document-name|Display Text]]` when needed
- Link to related concepts, decisions, and documents throughout content
- Create bidirectional links to build a knowledge graph

#### Tags
- **ALWAYS** include relevant tags at the bottom of documents
- Use consistent tag hierarchy:
  - Primary category: `#planning`, `#specs`, `#business`, `#meeting`, `#decision`
  - Project/topic: `#project-name`, `#feature-name`
  - Status: `#draft`, `#review`, `#approved`, `#archived`
  - Priority: `#high-priority`, `#medium-priority`, `#low-priority`
- Format: `**Tags**: #tag1 #tag2 #tag3`

#### Task Lists
- Use `- [ ]` for incomplete tasks
- Use `- [x]` for completed tasks
- Include assignee when relevant: `- [ ] Task description - @assignee`
- Include due dates: `- [ ] Task description - Due: YYYY-MM-DD`
- Use nested task lists for complex workflows

#### Mermaid Diagrams
- **ALWAYS** use Mermaid for visual representations when helpful
- Common diagram types to use:
  - Flowcharts for processes and decision trees
  - Gantt charts for project timelines
  - Sequence diagrams for interactions
  - Mind maps for brainstorming and concept mapping

## Document Templates & Formatting

### 1. Document Header Format
Every document should start with:
```markdown
# Document Title

**Created**: YYYY-MM-DD
**Last Updated**: YYYY-MM-DD
**Status**: [Draft/Review/Approved/Archived]
**Owner**: [Name or Role]

## Overview
[Brief description of document purpose and scope]
```

### 2. Meeting Notes Requirements
- **ALWAYS** use the meeting notes template
- Include all attendees (including AI assistants)
- Use task lists for action items with assignees and due dates
- Link to related documents and previous meetings
- Include Mermaid diagrams for complex discussions or workflows

### 3. Decision Records Requirements
- **ALWAYS** use the decision record template
- Include all options considered with pros/cons
- Use tables for option comparison when helpful
- Include implementation timeline with task lists
- Link to related decisions and supporting documents

### 4. Planning Documents Requirements
- Include Mermaid Gantt charts for timelines
- Use task lists for milestones and deliverables
- Link to related specifications and business documents
- Include risk assessment with mitigation strategies

## Mermaid Diagram Standards

### Flowcharts
```mermaid
flowchart TD
    A[Start] --> B{Decision}
    B -->|Yes| C[Action 1]
    B -->|No| D[Action 2]
    C --> E[End]
    D --> E
```

### Gantt Charts
```mermaid
gantt
    title Project Timeline
    dateFormat  YYYY-MM-DD
    section Phase 1
    Task 1           :a1, 2025-01-01, 30d
    Task 2           :after a1, 20d
    section Phase 2
    Task 3           :2025-02-01, 25d
```

### Mind Maps
```mermaid
mindmap
  root((Project))
    Planning
      Requirements
      Timeline
      Resources
    Implementation
      Development
      Testing
      Deployment
    Review
      Feedback
      Iteration
```

## Content Quality Standards

### 1. Completeness
- **ALWAYS** fill in all template sections or remove unused ones
- Include context and background information
- Provide clear next steps and action items
- Link to supporting materials and references

### 2. Clarity
- Use clear, concise language
- Define technical terms and acronyms
- Include examples when helpful
- Structure content logically with appropriate headings

### 3. Consistency
- Follow established naming conventions
- Use consistent terminology throughout
- Maintain consistent formatting and structure
- Apply tags consistently across similar documents

## Workflow Rules

### 1. Document Creation
- **ALWAYS** start with appropriate template from `05-templates/`
- Copy template to correct folder and rename appropriately
- Fill in all relevant sections
- Add appropriate tags and links
- Create initial commit with descriptive message

### 2. Document Updates
- Update "Last Updated" date when making changes
- Add changelog section for significant updates
- Update related documents and links as needed
- Commit changes with descriptive commit messages

### 3. Document Archival
- Move completed documents to `06-archive/` with appropriate subfolder
- Add "ARCHIVED" prefix to filename
- Update links in active documents
- Include archive reason and date in document header

## AI Assistant Guidelines

### When Creating New Documents
1. Ask which folder the document should go in if unclear
2. Use appropriate template from `05-templates/`
3. Include all required metadata and formatting
4. Add relevant tags and wikilinks
5. Include Mermaid diagrams when they add value
6. Create task lists for actionable items

### When Updating Existing Documents
1. Maintain existing structure and formatting
2. Update "Last Updated" date
3. Add new wikilinks to related content
4. Update task lists and completion status
5. Add changelog entry for significant changes

### When Analyzing or Reviewing
1. Check for consistency with these rules
2. Suggest improvements for clarity and completeness
3. Identify missing links or tags
4. Recommend Mermaid diagrams where helpful
5. Ensure proper folder organization

## File Naming Conventions

### General Rules
- Use lowercase letters only
- Use hyphens (-) instead of spaces or underscores
- Include dates in YYYY-MM-DD format when relevant
- Be descriptive but concise
- Use consistent prefixes for document types

### Examples
- Meeting notes: `2025-12-09-meeting-project-kickoff.md`
- Decision records: `2025-12-09-decision-database-selection.md`
- Project plans: `project-plan-mobile-app.md`
- Specifications: `api-specification-v2.md`
- Business docs: `stakeholder-analysis-q1.md`

## Quality Checklist

Before finalizing any document, ensure:
- [ ] Appropriate folder location
- [ ] Correct naming convention
- [ ] All template sections completed or removed
- [ ] Relevant wikilinks added
- [ ] Appropriate tags included
- [ ] Mermaid diagrams where helpful
- [ ] Task lists for actionable items
- [ ] Metadata complete (dates, status, owner)
- [ ] Clear and concise writing
- [ ] Proper markdown formatting
- [ ] Links to related documents

---

**Tags**: #meta #documentation-standards #windsurf-rules #obsidian
**Created**: 2025-12-09
**Last Updated**: 2025-12-09
