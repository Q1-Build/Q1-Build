# Portfolio Profile Guidelines

## Scope

These rules apply to the entire repository.

This repository is the public GitHub profile and portfolio landing page for
Q1-Build. Keep visitor-facing content in `README.md` and keep maintenance rules
in this file.

## Repository Purpose

- Present Q1-Build as a Unity and C# game developer.
- Show growth through completed projects and concrete technical contributions.
- Keep the profile easy to scan for recruiters, developers, and collaborators.
- Prefer evidence and specific contributions over broad technical claims.

## README Structure

Keep the main sections in this order:

1. Introduction
2. Recent Project
3. Core Stack & Practices
4. Featured Projects
5. Engineering Approach
6. Development Activity
7. Explore & Support

Do not add maintenance notes, writing rules, or internal checklists to
`README.md`.

## Recent Project

- Feature only the newest or currently most important project.
- Keep this section intentionally brief.
- Include one gameplay preview, a one-sentence description, exactly two concise
  contribution bullets, relevant technology tags, and a repository or demo
  link.
- Put full project details in the matching Featured Projects entry.
- When the featured project changes, update this section and verify that the
  previous project still appears under Featured Projects.

## Featured Projects

- Display projects from newest to oldest.
- Preserve project numbers as creation-order identifiers; do not renumber older
  projects when a new project is added.
- Use the following structure when the information is available:

```markdown
### NN. Project Name

Gameplay preview

Video or playable-demo link

One-sentence project description.

**Project Type**
Solo personal project or team project

**Genre**
Genre · Platform · Key characteristic

**Role & Contributions**

- Concrete contribution
- Concrete contribution
- Concrete contribution

**Technical Highlights**

- Problem, implementation choice, and result

**Repository**
Repository link or an explicit private-repository label
```

- Omit an unavailable optional field instead of adding an empty placeholder.
- Distinguish personal contributions from the team's overall work.
- For private repositories, provide public evidence when possible, such as a
  gameplay video, architecture diagram, sanitized code sample, or technical
  retrospective.

## Writing Conventions

- Write visitor-facing portfolio content in clear, concise English.
- Use consistent project names, capitalization, terminology, and punctuation.
- Prefer concrete verbs such as `designed`, `implemented`, `optimized`, and
  `refactored`.
- Avoid unsupported claims such as "high performance" or "clean architecture."
- When possible, describe technical work as problem, decision, and measurable
  result.
- Keep list items parallel in tone and grammatical structure.
- Expand uncommon abbreviations on first use.
- Do not duplicate detailed descriptions between Recent Project and Featured
  Projects.

## Unity and C# Presentation

- Keep Unity and C# as the primary technical identity of the profile.
- Use `csharp` for C# code fences.
- Code shown in the README must be syntactically valid or clearly labeled as
  pseudocode.
- List only technologies and practices that are supported by project work.
- Detailed Unity/C# source conventions belong in each game repository, not in
  this profile repository.

## Asset Conventions

- Store project media under `assets/projects/<project-name>/`.
- Use lowercase kebab-case for new directory and file names.
- Prefer predictable names such as `gameplay.gif`, `thumbnail.webp`, and
  `architecture.png`.
- Keep README gameplay previews at a consistent width of 640 pixels unless a
  different size materially improves readability.
- Optimize animated assets before committing them. Target 5 MB or less per
  preview when practical.
- Provide meaningful `alt` text for every image.
- Do not add the same media file to multiple locations.

## Links and Repository Labels

- Prefer links to a playable build, public repository, technical write-up, or
  gameplay video.
- Use descriptive link text instead of raw URLs.
- Label inaccessible repositories consistently as `Private Repository` or
  `Private Team Repository`.
- Verify every new or modified link before completing an update.

## Generated Content

- Do not manually edit files under `profile-3d-contrib/`.
- Treat `.github/workflows/profile-3d.yml` as the owner of those generated
  files.
- Do not treat files under `.git/`, including hook samples, as portfolio source
  files.
- Keep generated contribution updates separate from hand-authored portfolio
  changes when practical.

## Change Boundaries

- Preserve unrelated user changes in the working tree.
- Do not rename existing assets solely for style consistency unless every
  reference is updated in the same change.
- Do not add project facts, performance numbers, roles, or results that cannot
  be verified from user-provided or repository evidence.
- Do not commit or push unless the user explicitly requests it.

## Validation Checklist

After changing portfolio content:

1. Confirm the README section order remains intact.
2. Confirm Recent Project is concise and matches a Featured Projects entry.
3. Confirm project numbering and newest-to-oldest ordering.
4. Confirm image paths, alt text, and external links.
5. Confirm terminology and project names are consistent.
6. Run `git diff --check`.
7. Review `git diff` and `git status --short` for unintended changes.
