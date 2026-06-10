# 📚 Documentation Guide - English

Welcome to the **AgroVision** documentation guide! This document explains how to structure, write, and maintain project documentation.

## Table of Contents

- [Documentation Structure](#documentation-structure)
- [Writing Standards](#writing-standards)
- [Types of Documentation](#types-of-documentation)
- [Best Practices](#best-practices)
- [Documentation Versioning](#documentation-versioning)

## Documentation Structure

### Folder Hierarchy

```
docs/
├── README.md                 # Documentation index
├── getting-started.en.md     # Getting started guide (EN)
├── data-guide.en.md          # Data guide (EN)
├── documentation-guide.en.md # This document
├── api/
│   ├── endpoints.md
│   └── authentication.md
├── guides/
│   ├── setup.md
│   └── deployment.md
└── tutorials/
    ├── first-analysis.md
    └── data-visualization.md
```

## Writing Standards

### 1. Title Structure

Always use consistent Markdown headers:

```markdown
# Main Title (H1)
## Section (H2)
### Subsection (H3)
#### Details (H4)
```

### 2. Tone and Voice

- **Friendly**: Use accessible language
- **Clear**: Avoid technical jargon without explanation
- **Concise**: Get straight to the point
- **Inclusive**: Consider diverse audiences (farmers, researchers, etc.)

### 3. Formatting

Use markdown consistently:

```markdown
- **Bold** for important terms
- `code` for filenames/functions
- [Links](url) for references
- > Blockquotes for highlights
- ```code blocks``` for examples
```

## Types of Documentation

### 1. Quick Start Documentation

**Purpose**: Get users started in 5 minutes

**Example structure**:
- Prerequisites
- Installation
- First use
- Next steps

### 2. How-To Guides

**Purpose**: Solve a specific problem

**Example structure**:
- Problem statement
- Step-by-step solution
- Practical examples
- Tips and tricks

### 3. Reference

**Purpose**: Complete documentation of APIs/functions

**Example structure**:
- Description
- Parameters
- Usage examples
- Error cases

### 4. Conceptual Explanations

**Purpose**: Education on ideas/concepts

**Example structure**:
- Context
- Detailed explanation
- Real-world examples
- Additional resources

## Best Practices

### 1. Write for Your Audience

Consider who is reading:

- **For Farmers**: Use practical examples, avoid heavy jargon
- **For Researchers**: Include scientific references, methodology
- **For Developers**: Use code examples, technical details
- **For General Community**: Simple and accessible language

### 2. Use Real Examples

```markdown
❌ Bad: "Enter the data"
✅ Good: "Copy your CSV data to the `data/raw/` folder and run:"
```

### 3. Keep Documentation Updated

- Update docs when code changes
- Check links regularly
- Review and improve continuously

### 4. Include Images and Diagrams

```markdown
![Image Description](path/to/image.png)
```

### 5. Use Tables for Comparisons

```markdown
| Resource | Description | Audience |
|----------|-------------|----------|
| Data Guide | How to work with data | Everyone |
| API Ref | Technical reference | Developers |
```

### 6. Add Warnings and Tips

```markdown
> **⚠️ Warning**: Make sure to backup first
> **💡 Tip**: Use environment variables for passwords
> **ℹ️ Note**: This feature is in beta
```

## Documentation Versioning

### Version Maintenance

1. **Main Docs**: Always reflect the most recent version
2. **Release Docs**: Archived by version if needed
3. **Changelog**: Record important documentation changes

### When to Update

- New features
- API changes
- Bug fixes
- Performance improvements
- Structure changes

## Documentation Review

### Pull Request Checklist

- [ ] Clear and descriptive titles
- [ ] Functional and tested examples
- [ ] Working links
- [ ] Consistent formatting
- [ ] Review by another maintainer
- [ ] No typos

## Additional Resources

- 📖 [Full Documentation](../README.en.md)
- 🤝 [Contributing](../CONTRIBUTING.md)
- 💬 [Discussions](../../discussions)

---

**Versions in other languages:** [🇧🇷 Português](./documentation-guide.pt.md) | [🇪🇸 Español](./documentation-guide.es.md)

Have questions about documentation? [Open a Discussion](../../discussions)
