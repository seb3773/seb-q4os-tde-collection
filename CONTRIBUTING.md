# Contributing to Q4OS TDE Collection

First off, thank you for considering contributing to the Q4OS TDE Collection! 🎉

This repository thrives on community contributions. Whether you're adding a new theme, fixing a typo, or sharing a useful resource, your help is appreciated.

## 📋 Table of Contents

- [How Can I Contribute?](#how-can-i-contribute)
- [Contribution Guidelines](#contribution-guidelines)
- [Adding Resources](#adding-resources)
- [Reporting Issues](#reporting-issues)
- [Style Guide](#style-guide)
- [Commit Messages](#commit-messages)

---

## 🤝 How Can I Contribute?

### 1. Add New Resources

You can contribute:
- **Themes**: Color schemes, Dekorator themes, complete desktop themes
- **Visual Resources**: Cursors, icons, fonts, wallpapers, Plymouth themes
- **Tools & Scripts**: Useful utilities for Q4OS/TDE
- **Documentation**: Tutorials, guides, tips & tricks
- **Media**: Artwork, screenshots, videos
- **Reviews & Articles**: Links to Q4OS/TDE reviews, blog posts, videos

### 2. Improve Existing Content

- Fix broken links
- Update outdated information
- Add missing previews or screenshots
- Improve documentation clarity
- Translate content to other languages

### 3. Report Issues

- Broken links or downloads
- Missing resources
- Incorrect information
- Suggestions for improvements

---

## 📝 Contribution Guidelines

### General Rules

1. **Quality over quantity**: Ensure resources are tested and working
2. **Respect licenses**: Only contribute resources you have the right to share
3. **Be descriptive**: Provide clear descriptions and proper attribution
4. **Stay on topic**: Keep contributions relevant to Q4OS and Trinity Desktop

### Before Contributing

- Check if the resource already exists in the collection
- Test the resource on Q4OS (preferably latest stable version)
- Verify you have permission to share the resource
- Prepare any necessary files (previews, screenshots, archives)

---

## 📦 Adding Resources

### Step-by-Step Process

1. **Fork the repository**
   ```bash
   # Click the "Fork" button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/seb-q4os-tde-collection.git
   cd seb-q4os-tde-collection
   ```

3. **Create a new branch**
   ```bash
   git checkout -b add-new-resource
   ```

4. **Add your resource**
   - Place files in the appropriate directory
   - Follow the naming conventions (see below)
   - Add preview images if applicable

5. **Update documentation**
   - Add entry to the relevant `.md` file
   - Include description, preview, and download link
   - Follow the existing format

6. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add [resource name] to [category]"
   ```

7. **Push to your fork**
   ```bash
   git push origin add-new-resource
   ```

8. **Create a Pull Request**
   - Go to the original repository on GitHub
   - Click "New Pull Request"
   - Describe what you're adding and why

---

## 🎨 Adding Specific Resource Types

### Color Schemes

**Location**: `assets/color schemes/`

**Requirements**:
- File format: `.kcsrc`
- Preview image: PNG, 800x600px minimum
- Place preview in `assets/color_previews/`

**Example entry in `color_schemes.md`**:
```markdown
| **Your Scheme Name** | ![](./assets/color_previews/YourScheme.png) | [Download](./assets/color%20schemes/YourScheme.kcsrc) |
```

### Dekorator Themes

**Location**: `assets/dekorator/`

**Requirements**:
- Archive format: `.tar`, `.tar.gz`, or `.zip`
- Preview image: PNG showing window decoration
- Place preview in `assets/dekorator_previews/`

### Fonts

**Location**: `assets/fonts/`

**Requirements**:
- File format: `.ttf` or `.otf`
- Preview image: PNG showing font sample
- Place preview in `assets/previews/`
- Include license information if available

### Icons & Cursors

**Location**: `assets/icons/` or `assets/cursors/`

**Requirements**:
- Archive format: `.tar.gz`, `.zip`, or directory
- Preview image showing representative samples
- Installation instructions if non-standard

### Articles & Reviews

**Location**: `reviews_press_blogs.md`

**Requirements**:
- Article title and author
- Publication date
- Language indicator (🇫🇷, 🇩🇪, 🇪🇸, etc.)
- Brief description (1-2 sentences)
- Working link to article
- Optional: Archive in `assets/archives/articles/`

**Example**:
```markdown
- **📄 Article Title** — *Source* (YYYY-MM-DD) 🇫🇷 *French*
  Brief description of the article content.
  🔗 [Read article](https://example.com)
  📦 [Archive](assets/archives/articles/YYYY-MM-source-title.md)
```

### Tools & Projects

**Location**: README.md under appropriate section

**Requirements**:
- Link to GitHub repository or download
- Clear description of functionality
- Installation/usage instructions
- Compatibility information (Q4OS version, TDE version)

---

## 🐛 Reporting Issues

### Bug Reports

When reporting a bug, please include:
- **Description**: What's wrong?
- **Steps to reproduce**: How can we see the problem?
- **Expected behavior**: What should happen?
- **Actual behavior**: What actually happens?
- **Environment**: Q4OS version, TDE version, hardware

### Feature Requests

When suggesting a feature:
- **Description**: What would you like to see?
- **Use case**: Why is this useful?
- **Examples**: Similar implementations elsewhere?

---

## 📐 Style Guide

### File Naming Conventions

- **Use descriptive names**: `windows10-theme.kcsrc` not `theme1.kcsrc`
- **Lowercase with hyphens**: `my-awesome-theme` not `My_Awesome_Theme`
- **No spaces**: Use hyphens or underscores
- **Version numbers**: Include if relevant: `theme-v2.0.tar.gz`

### Markdown Formatting

- Use consistent heading levels
- Include emojis for visual appeal (but don't overdo it)
- Use tables for structured data
- Add line breaks for readability
- Use code blocks for commands and code

### Image Guidelines

- **Format**: PNG preferred, JPG acceptable
- **Size**: Reasonable file size (compress if needed)
- **Dimensions**: Minimum 400px width for previews
- **Naming**: Match the resource name

---

## 💬 Commit Messages

### Format

```
<type>: <subject>

<body (optional)>
```

### Types

- `add`: Adding new resources
- `update`: Updating existing content
- `fix`: Fixing errors or broken links
- `docs`: Documentation changes
- `style`: Formatting, no content change
- `remove`: Removing outdated content

### Examples

```bash
add: Windows 11 color scheme with preview

fix: broken link in reviews_press_blogs.md

update: Q4OS 6.1 documentation

docs: improve installation instructions for fonts
```

---

## 🌍 Translation Contributions

We welcome translations of documentation!

**Priority documents**:
- README.md
- CONTRIBUTING.md
- Installation guides

**Process**:
1. Create a new file: `README.fr.md`, `README.de.md`, etc.
2. Translate the content
3. Keep formatting and structure consistent
4. Submit a pull request

---

## ✅ Checklist Before Submitting

- [ ] Resource is tested and working on Q4OS
- [ ] Files are in the correct directory
- [ ] Preview images are included (if applicable)
- [ ] Documentation is updated
- [ ] Links are working
- [ ] Commit messages are clear
- [ ] No duplicate content
- [ ] License/attribution is respected

---

## 🎯 What We're Looking For

**High Priority**:
- Complete desktop themes (coordinated color schemes + dekorator + icons)
- Wallpaper collections
- Conky configurations
- Useful scripts and utilities
- Video tutorials
- Translations

**Always Welcome**:
- Bug fixes
- Documentation improvements
- New themes and visual resources
- Community showcases

---

## 📞 Questions?

- Open an issue for questions
- Check existing issues and pull requests first
- Be patient and respectful

---

## 🙏 Thank You!

Every contribution, no matter how small, helps make Q4OS and Trinity Desktop better for everyone. We appreciate your time and effort!

**Happy contributing!** 🚀
