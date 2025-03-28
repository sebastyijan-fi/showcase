# Contributing to the Vibecoders Showcase

Thank you for your interest in adding your project to the [Vibecoders.eu Showcase](https://vibecoders.eu/showcase)! Please follow these steps to submit your project via a Pull Request (PR) using a JSON file.

## How to Submit

The easiest way to submit your project is using the GitHub web interface.

**Method 1: Using the GitHub Web Interface (Recommended)**

1.  **Navigate to the Showcase Folder:** Go to the `showcase` folder within this repository: [https://github.com/vibecoders/showcase/tree/main/showcase](https://github.com/vibecoders/showcase/tree/main/showcase)
    *(Note: If the 'showcase' folder doesn't exist yet, you might need to create it first, or the first person submitting can create it during the 'Add file' step below).*
2.  **Add File:** Click the "Add file" button (usually near the top right) and select "Create new file".
3.  **Name Your File:** In the box that says `showcase/` followed by "Name your file...", type the filename for your project. Use a unique slug based on your project name, followed by `.json`. Use only lowercase letters, numbers, and hyphens (e.g., `my-awesome-app.json`). The full path should look like `showcase/my-awesome-app.json`.
4.  **Add Content:**
    * Copy the contents of the `template.json` file (located in the root of this repository).
    * Paste the template content into the large text editing box on the GitHub page.
    * **Edit the content**, replacing the placeholder values with your project's actual details. Ensure it is valid JSON (see **JSON Data Requirements** below).
5.  **Propose New File:** Scroll down below the editor. Add a short commit message (e.g., "Add showcase: My Awesome App") and optionally a description. Click the "Propose new file" button.
6.  **Open Pull Request:** GitHub will typically take you directly to a page to open a Pull Request. Review the details and click "Create pull request".

**Method 2: Using Git Locally (Alternative)**

If you prefer using Git on your command line:

1.  **Fork this Repository:** Create your own copy by clicking "Fork".
2.  **Clone Your Fork:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/showcase.git](https://github.com/YOUR_USERNAME/showcase.git)
    cd showcase
    ```
3.  **Create a Branch:**
    ```bash
    git checkout -b add-my-project-name
    ```
4.  **Create & Edit JSON File:**
    * Ensure a `showcase` directory exists. If not, create it: `mkdir showcase`
    * Copy the `template.json` file into the `showcase` directory.
    * Rename the copied file inside the `showcase` directory to `showcase/your-project-slug.json` (e.g., `showcase/my-awesome-app.json`).
    * Edit the file (`showcase/your-project-slug.json`), filling in the JSON fields accurately. Ensure it is valid JSON.
5.  **Commit Changes:**
    ```bash
    # Make sure you add the file inside the showcase directory!
    git add showcase/your-project-slug.json
    git commit -m "feat: Add showcase submission for [Your Project Name]"
    ```
6.  **Push to Your Fork:**
    ```bash
    git push origin add-my-project-name
    ```
7.  **Open a Pull Request:** Go to the main `vibecoders/showcase` repository page on GitHub and open a Pull Request from your branch.

## JSON Data Requirements

Your submission file (`showcase/your-project-slug.json`) **must** contain a single JSON object with specific key-value pairs defining your project's details.

* Please refer to the `template.json` file in the root of this repository for the exact structure, field names, and example values required.
* A detailed explanation of each field (Required: `title`, `submitter_github`, `project_url`, `image_url`, `description`; Recommended: `repo_url`, `vibecoders_stack_url`, `related_tools`, `tags`, `based_in`) was provided previously.
* **Important JSON Syntax:**
    * All keys (field names) must be enclosed in double quotes (e.g., `"title"`).
    * All string values must be enclosed in double quotes (e.g., `"Your Project Name"`).
    * Lists/arrays use square brackets `[]`, with values inside (e.g., `["tag1", "tag2"]`).
    * Separate key-value pairs with commas `,`.
    * Do **not** include a trailing comma after the last key-value pair in the object.
    * You can use online JSON validators to check your file before submitting.
* Ensure all required fields are present and accurately filled with the correct data type. The placeholder comment keys (like `"_comment_//_Required_Fields"`) in the template should ideally be removed in your final submission.

## Image Guidelines (`image_url`)

* You **must** provide a direct URL for the `"image_url"` field, pointing to an image representing your project (e.g., a screenshot).
* Host the image yourself (e.g., on your project's CDN, a public folder) or use a reliable image hosting service. Do **not** link to temporary URLs or pages *containing* the image; link directly to the image file itself (e.g., ending in `.jpg`, `.png`, `.webp`).
* **Recommendations:**
    * **Aspect Ratio:** Aim for 16:9 (e.g., 1200x675 pixels) if possible, for consistency.
    * **Format:** Use JPG, PNG, or ideally WebP for better compression.
    * **Size:** Optimize your image! Aim for **under 300KB**. Use tools like [TinyPNG](https://tinypng.com/) or [Squoosh](https://squoosh.app/).
* Broken or invalid image URLs may delay or prevent your submission from being merged.

## Review Process

* We (the maintainers) will review submitted Pull Requests.
* We check for valid JSON formatting, completeness of required fields, validity of URLs (project and image), and relevance (e.g., connection to EU tech, privacy focus, use of relevant tools). We also check to ensure submissions are not spam.
* We aim to review PRs reasonably quickly, but please allow some time.
* We may ask for changes via comments on your Pull Request before merging.

## Licensing

By submitting content (the information within your submitted `.json` file) via a Pull Request to this repository, you agree to license that submitted content under the terms specified in the [LICENSE](LICENSE) file of this repository (e.g., CC-BY-4.0). This allows Vibecoders.eu to display the information. You retain all rights to your actual project code and the linked image itself.

## Code of Conduct

Please note that this project aims to follow a positive and constructive community standard. By participating, you agree to engage respectfully. (Consider adding a formal `CODE_OF_CONDUCT.md` file and linking it here if desired).
