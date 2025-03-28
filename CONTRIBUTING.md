# Contributing to the Vibecoders Showcase

Thank you for your interest in adding your project to the [Vibecoders.eu Showcase](https://vibecoders.eu/showcase)! Please follow these steps to submit your project via a Pull Request (PR).

## How to Submit

1.  **Fork this Repository:** Click the "Fork" button at the top right of this page.
2.  **Clone Your Fork:** Clone your forked repository to your local machine.
    ```bash
    git clone [https://github.com/YOUR_USERNAME/showcase.git](https://www.google.com/search?q=https://github.com/YOUR_USERNAME/showcase.git)
    cd showcase
    ```
3.  **Create a Branch:** Create a new branch for your submission. Use a descriptive name (e.g., `add-my-project-name`).
    ```bash
    git checkout -b add-my-project-name
    ```
4.  **Create a Markdown File:**
    * Copy the `template.md` file.
    * Rename it to `your-project-slug.md` in the root directory. Use lowercase letters, numbers, and hyphens only (e.g., `my-awesome-app.md`).
    * **Do NOT** create subdirectories for your file.
5.  **Edit the File:** Fill in the front matter fields in your new Markdown file (`your-project-slug.md`). See **Front Matter Requirements** below.
6.  **Commit Changes:** Stage and commit your new file.
    ```bash
    git add your-project-slug.md
    git commit -m "feat: Add showcase submission for [Your Project Name]"
    ```
7.  **Push to Your Fork:** Push your branch to your forked repository on GitHub.
    ```bash
    git push origin add-my-project-name
    ```
8.  **Open a Pull Request:** Go to the original `vibecoders/showcase` repository on GitHub. You should see a prompt to create a Pull Request from your new branch. Click it, review the changes, and submit the PR.

## Front Matter Requirements

Your Markdown file (`your-project-slug.md`) **must** contain the following YAML front matter fields:

```yaml
---
# ----------- Required Fields -----------
title: "Your Project Name"              # Max 60 characters recommended
submitter_github: "your-github-username" # Your GitHub username (no @)
project_url: "[https://your-project-live-url.com](https://your-project-live-url.com)" # Must be a live, accessible URL
image_url: "[https://your-image-host.com/image.jpg](https://your-image-host.com/image.jpg)" # Direct URL to a screenshot/image (see Image Guidelines below)
description: "A concise (1-2 sentences, max 160 chars) description of your project."

# ----------- Recommended Fields -----------
repo_url: "[https://github.com/your/repo](https://github.com/your/repo)"        # Optional: Link to the source code repository
# Strongly encouraged if your project uses tools listed on Vibecoders.eu!
vibecoders_stack_url: "[https://vibecoders.eu/stack/your-stack-slug-or-id](https://vibecoders.eu/stack/your-stack-slug-or-id)"
# List slugs of specific tools from vibecoders.eu used in your project
related_tools: ["baserow", "plausible-analytics", "hetzner-cloud"]
# General tags (lowercase, hyphenated if needed)
tags: ["saas", "analytics", "web-app", "open-source", "privacy"]
based_in: "Finland"                           # Optional: Primary country focus or location

# ----------- Optional Markdown Body -----------
---

## Optional Details Below

You can add more Markdown content below the front matter if you want to provide extra details, but keep it concise. The main focus will be the linked project and the front matter details.
