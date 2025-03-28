# Contributing to the Vibecoders Showcase

Thank you for your interest in adding your project to the [Vibecoders.eu Showcase](https://vibecoders.eu/showcase)! Please follow these steps to submit your project via a Pull Request (PR).

## How to Submit

1.  **Fork this Repository:** Click the "Fork" button at the top right of this page.
2.  **Clone Your Fork:** Clone your forked repository to your local machine.
    ```bash
    git clone [https://github.com/YOUR_USERNAME/showcase.git](https://github.com/YOUR_USERNAME/showcase.git)
    cd showcase
    ```
3.  **Create a Branch:** Create a new branch for your submission. Use a descriptive name (e.g., `add-my-project-name`).
    ```bash
    git checkout -b add-my-project-name
    ```
4.  **Create a Markdown File:**
    * Copy the `template.md` file from the root of the repository.
    * Rename the copied file to `your-project-slug.md` in the root directory. Use only lowercase letters, numbers, and hyphens for the slug (e.g., `my-awesome-app.md`).
    * **Do NOT** create subdirectories for your file. Place it directly in the root.
5.  **Edit the File:** Fill in the YAML front matter fields accurately in your new Markdown file (`your-project-slug.md`). See **Front Matter Requirements** below for details on each field and refer to `template.md` for the exact structure.
6.  **Commit Changes:** Stage and commit your new file with a clear commit message.
    ```bash
    git add your-project-slug.md
    git commit -m "feat: Add showcase submission for [Your Project Name]"
    ```
7.  **Push to Your Fork:** Push your new branch and commit to your forked repository on GitHub.
    ```bash
    git push origin add-my-project-name
    ```
8.  **Open a Pull Request:** Go back to the main `vibecoders/showcase` repository page on GitHub. You should see a prompt suggesting you create a Pull Request from the branch you just pushed. Click it, review your changes, add any relevant comments, and submit the Pull Request.

## Front Matter Requirements

Your Markdown file (`your-project-slug.md`) **must** start with a YAML front matter block enclosed in `---` delimiters. This block contains key-value pairs defining your project's details.

Please refer to the `template.md` file in this repository for the exact structure and field names required. A detailed explanation of each field (Required: `title`, `submitter_github`, `project_url`, `image_url`, `description`; Recommended: `repo_url`, `vibecoders_stack_url`, `related_tools`, `tags`, `based_in`) was provided previously and should be followed. Ensure all required fields are present and accurately filled.

## Image Guidelines (`image_url`)

* You **must** provide a direct URL (`image_url`) to an image representing your project (e.g., a screenshot).
* Host the image yourself (e.g., on your project's CDN, a public folder) or use a reliable image hosting service. Do **not** link to temporary URLs or pages *containing* the image; link directly to the image file itself (e.g., ending in `.jpg`, `.png`, `.webp`).
* **Recommendations:**
    * **Aspect Ratio:** Aim for 16:9 (e.g., 1200x675 pixels) if possible, for consistency.
    * **Format:** Use JPG, PNG, or ideally WebP for better compression.
    * **Size:** Optimize your image! Aim for **under 300KB**. Use tools like [TinyPNG](https://tinypng.com/) or [Squoosh](https://squoosh.app/).
* Broken or invalid image URLs may delay or prevent your submission from being merged.

## Review Process

* We (the maintainers) will review submitted Pull Requests.
* We check for correct formatting, completeness of required fields, validity of URLs (project and image), and relevance (e.g., connection to EU tech, privacy focus, use of relevant tools). We also check to ensure submissions are not spam.
* We aim to review PRs reasonably quickly, but please allow some time.
* We may ask for changes via comments on your Pull Request before merging.

## Licensing

By submitting content (the information within your submitted `.md` file) via a Pull Request to this repository, you agree to license that submitted content under the terms specified in the [LICENSE](LICENSE) file of this repository (e.g., CC-BY-4.0). This allows Vibecoders.eu to display the information. You retain all rights to your actual project code and the linked image itself.

## Code of Conduct

Please note that this project aims to follow a positive and constructive community standard. By participating, you agree to engage respectfully. (Consider adding a formal `CODE_OF_CONDUCT.md` file and linking it here if desired).
