# CLAUDE.md - AI Assistant Guide

This document provides comprehensive guidance for AI assistants working with this repository. It explains the codebase structure, development workflows, and key conventions to follow.

## Repository Overview

This is a **special GitHub repository** named `.github` that serves as a centralized location for community health files and GitHub profile configuration for the user **charge0315**.

### Purpose

GitHub recognizes `.github` repositories as special repositories that provide:
- **Community health files** (CODE_OF_CONDUCT.md, CONTRIBUTING.md, SECURITY.md, etc.) that automatically apply to all public repositories owned by the user
- **GitHub profile README** (profile/README.md) displayed on the user's GitHub profile page
- **Issue and PR templates** that can be shared across repositories

## Repository Structure

```
.github/
├── .github/
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.yml          # Bug report issue template
│       ├── feature_request.yml     # Feature request issue template
│       └── config.yml              # Issue template configuration
├── profile/
│   └── README.md                   # GitHub profile README
├── CODE_OF_CONDUCT.md              # Community code of conduct
├── CONTRIBUTING.md                 # Contribution guidelines
├── FUNDING.yml                     # Sponsorship/funding configuration
├── README.md                       # Repository description
├── SECURITY.md                     # Security policy
└── SUPPORT.md                      # Support documentation
```

## File Descriptions

### Community Health Files

#### CODE_OF_CONDUCT.md
- **Purpose**: Defines community standards and behavior expectations
- **Standard**: Contributor Covenant v2.0
- **Applies to**: All public repositories owned by charge0315
- **Key sections**:
  - Our Pledge (harassment-free experience)
  - Our Standards (acceptable/unacceptable behavior)
  - Enforcement Responsibilities
  - Scope and attribution

#### CONTRIBUTING.md
- **Purpose**: Guidelines for contributing to projects
- **Contains**:
  - How to report issues
  - Submitting changes workflow (fork → branch → commit → PR)
  - Code style expectations
  - Testing requirements
  - Reference to Code of Conduct

#### SECURITY.md
- **Purpose**: Security vulnerability reporting and handling
- **Key points**:
  - Do NOT report vulnerabilities via public GitHub issues
  - Email maintainers directly with vulnerability details
  - 48-hour response time commitment
  - Responsible disclosure expectations

#### SUPPORT.md
- **Purpose**: Help users get support
- **Contains**:
  - Documentation references
  - Issue creation guidelines
  - Discussion forum references
  - Best practices for asking questions

#### FUNDING.yml
- **Purpose**: Configure repository sponsorship options
- **Current state**: All funding platforms commented out
- **Available platforms**: GitHub Sponsors, Patreon, Open Collective, Ko-fi, etc.

### Issue Templates

#### .github/ISSUE_TEMPLATE/bug_report.yml
- **Type**: Structured YAML issue form
- **Label**: Automatically adds "bug" label
- **Fields**:
  - Bug Description (required)
  - Steps to Reproduce (required)
  - Expected Behavior (required)
  - Actual Behavior (required)
  - Environment (optional)
  - Screenshots (optional)
  - Additional Context (optional)

#### .github/ISSUE_TEMPLATE/feature_request.yml
- **Type**: Structured YAML issue form
- **Label**: Automatically adds "enhancement" label
- **Fields**:
  - Problem Statement (required)
  - Proposed Solution (required)
  - Alternatives Considered (optional)
  - Additional Context (optional)
  - Priority dropdown (Low/Medium/High/Critical)
  - Contribution willingness checkbox

#### .github/ISSUE_TEMPLATE/config.yml
- **Purpose**: Issue template configuration
- **Settings**:
  - `blank_issues_enabled: false` - Disables blank issues
  - Contact links for Documentation and Discussions

### Profile Files

#### profile/README.md
- **Purpose**: User's GitHub profile page
- **Content sections**:
  - Personal introduction
  - Technologies & tools (badges for Python, JavaScript, React, Docker, etc.)
  - GitHub statistics and graphs
  - Featured projects
  - Blog posts (placeholder)
  - Social media links
- **Styling**: Uses shields.io badges, GitHub stats widgets, centered layout

#### README.md
- **Current content**: ".github 新規作成" (New creation in Japanese)
- **Purpose**: Brief repository description
- **Note**: Could be expanded to explain the repository's purpose

## Development Workflows

### Making Changes to Community Health Files

When modifying community health files:

1. **Understand the impact**: Changes affect ALL public repositories
2. **Review carefully**: These files set community standards
3. **Follow conventions**:
   - Use clear, professional language
   - Maintain existing structure and formatting
   - Keep content concise and actionable
4. **Test templates**: For issue templates, verify YAML syntax is valid

### Updating Issue Templates

1. **YAML syntax**: Strictly validate before committing
2. **Required fields**: Balance between gathering info and user friction
3. **Labels**: Ensure labels exist in repositories or will be auto-created
4. **Testing**: Create test issues to verify template functionality

### Modifying the Profile README

1. **Visual consistency**: Maintain the Tokyo Night theme and centered layout
2. **Badges and widgets**: Ensure all external services (shields.io, vercel.app) URLs are correct
3. **Personal information**: Update placeholders with actual information
4. **Links**: Verify all URLs are functional

### Git Workflow

Standard git workflow for this repository:

```bash
# Create feature branch
git checkout -b feature/description

# Make changes
# ... edit files ...

# Commit with clear messages
git add .
git commit -m "type: clear description of changes"

# Push to origin
git push -u origin feature/description

# Create pull request (if applicable)
```

## Key Conventions for AI Assistants

### File Modification Guidelines

1. **Community Health Files**
   - **DO**: Maintain professional, inclusive language
   - **DO**: Follow Contributor Covenant standards for CODE_OF_CONDUCT.md
   - **DO**: Keep security reporting instructions clear and private
   - **DON'T**: Make breaking changes without user approval
   - **DON'T**: Remove important sections without discussion

2. **Issue Templates**
   - **DO**: Validate YAML syntax before committing
   - **DO**: Include helpful placeholder text
   - **DO**: Balance required vs optional fields
   - **DON'T**: Create overly complex forms that discourage reporting
   - **DON'T**: Forget to update labels if changing label assignments

3. **Profile README**
   - **DO**: Maintain visual consistency (theme, alignment, badges)
   - **DO**: Update statistics widgets with correct username
   - **DO**: Ensure all external links are functional
   - **DON'T**: Use placeholders in production (replace with actual info)
   - **DON'T**: Break the centered layout or visual theme

### Code Quality Standards

1. **Markdown**:
   - Use consistent heading levels
   - Include blank lines between sections
   - Use proper link formatting: `[text](url)`
   - Validate markdown syntax

2. **YAML**:
   - Indent with 2 spaces
   - Validate syntax before committing
   - Quote strings containing special characters
   - Follow GitHub's issue form schema

3. **File Organization**:
   - Keep files in their designated directories
   - Use clear, descriptive filenames
   - Maintain alphabetical ordering where applicable

### Security Considerations

1. **Never commit**:
   - Personal email addresses (unless intentionally public)
   - API keys or tokens
   - Private repository information
   - Sensitive user data

2. **Security reporting**:
   - Keep SECURITY.md instructions clear
   - Emphasize private reporting channels
   - Don't disclose vulnerabilities in commits

### Communication Style

When working with this repository:

1. **Commit messages**:
   - Use conventional commit format: `type: description`
   - Types: `feat`, `fix`, `docs`, `style`, `refactor`, `chore`
   - Example: `docs: update contributing guidelines`

2. **Documentation**:
   - Write in clear, simple English
   - Use active voice
   - Be concise but complete
   - Include examples where helpful

3. **Issue templates**:
   - Use welcoming, encouraging language
   - Provide clear instructions
   - Include helpful placeholders

## Common Tasks

### Adding a New Issue Template

1. Create new YAML file in `.github/ISSUE_TEMPLATE/`
2. Follow this structure:
```yaml
name: Template Name
description: Template description
title: "[PREFIX]: "
labels: ["label1", "label2"]
body:
  - type: markdown
    attributes:
      value: |
        Introduction text
  - type: textarea
    id: unique_id
    attributes:
      label: Field Label
      description: Field description
    validations:
      required: true
```
3. Update `config.yml` if needed
4. Test the template by creating an issue

### Updating Profile Statistics

The profile README uses external widgets that automatically update. To change the theme or style:

1. Locate the widget URL (e.g., `github-readme-stats.vercel.app`)
2. Modify query parameters:
   - `theme=tokyonight` - Changes color scheme
   - `hide_border=true` - Removes borders
   - `count_private=true` - Includes private repos
3. Verify the new URL renders correctly

### Enabling Funding

To enable sponsorship options in FUNDING.yml:

1. Uncomment the relevant platform line
2. Replace the placeholder with your username/URL
3. Example: `github: charge0315`
4. Commit and push changes
5. "Sponsor" button will appear on repositories

## Best Practices

### For AI Assistants

1. **Read before modifying**: Always read existing files completely before making changes
2. **Preserve intent**: Maintain the original purpose and tone of files
3. **Validate syntax**: Especially for YAML files, validate before committing
4. **Explain changes**: Provide clear commit messages and explanations
5. **Ask when uncertain**: If a change could have broad impact, ask the user first
6. **Test templates**: For issue templates, verify they work as expected
7. **Maintain consistency**: Keep formatting, style, and conventions consistent
8. **Consider scope**: Remember changes to community files affect all repos

### For Repository Maintenance

1. **Regular updates**:
   - Review and update contact information
   - Ensure external links remain functional
   - Update profile README with current projects

2. **Template effectiveness**:
   - Monitor if templates collect useful information
   - Adjust required/optional fields based on usage
   - Update templates as project needs evolve

3. **Documentation clarity**:
   - Keep instructions clear and up-to-date
   - Remove placeholder text before going public
   - Ensure consistency across all community files

## Technical Details

### GitHub Special Repositories

The `.github` repository is special because:

1. **Automatic fallback**: If a public repository doesn't have its own community health files, GitHub automatically uses files from this repository
2. **Profile README**: The `profile/README.md` file is displayed on the user's profile
3. **Organization-wide**: For organization accounts, this can provide default files for all repos

### File Precedence

When GitHub looks for community health files:

1. First checks the repository itself (e.g., `repo/CODE_OF_CONDUCT.md`)
2. Then checks `.github` repository (e.g., `.github/CODE_OF_CONDUCT.md`)
3. For organizations, checks `.github/.github/` directory

### Supported Community Health Files

Files that automatically apply across repositories:
- CODE_OF_CONDUCT.md
- CONTRIBUTING.md
- FUNDING.yml
- GOVERNANCE.md
- SECURITY.md
- SUPPORT.md
- Issue and PR templates

## Troubleshooting

### Issue Templates Not Appearing

1. Check YAML syntax is valid
2. Verify files are in `.github/ISSUE_TEMPLATE/` directory
3. Ensure `config.yml` doesn't have conflicting settings
4. Clear browser cache and reload

### Profile README Not Updating

1. Ensure file is at `profile/README.md` (exact path)
2. Verify repository is named exactly `.github`
3. Check repository visibility is public
4. Wait a few minutes for GitHub to refresh

### Community Files Not Applying

1. Verify repository is public (community files don't apply to private repos)
2. Check file names match exactly (case-sensitive)
3. Ensure repository is named `.github` (user) or `.github/.github/` (org)

## Resources

### Official Documentation

- [GitHub Community Health Files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [GitHub Issue Template Syntax](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms)
- [GitHub Profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [Contributor Covenant](https://www.contributor-covenant.org/)

### Useful Tools

- [shields.io](https://shields.io/) - Badge generator
- [GitHub Stats](https://github.com/anuraghazra/github-readme-stats) - Profile statistics widgets
- [YAML Validator](https://www.yamllint.com/) - Validate YAML syntax
- [Markdown Validator](https://www.markdownlint.com/) - Check markdown formatting

## Version History

- **2025-11-16**: Initial CLAUDE.md created with comprehensive documentation

## Contact

For questions about this repository structure or conventions:
- Email: charge0315@gmail.com
- GitHub: [@charge0315](https://github.com/charge0315)

---

**Note**: This document is intended for AI assistants to understand the repository structure and conventions. Keep it updated as the repository evolves.
