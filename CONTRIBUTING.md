## How to Submit

You can submit your project using either the simpler GitHub web interface or the standard Git command-line workflow.

**Method 1: Using the GitHub Web Interface (Recommended for single file submissions)**

1.  **Navigate to the Repository:** Go to the main page of the `vibecoders/showcase` repository: [https://github.com/vibecoders/showcase](https://github.com/vibecoders/showcase)
2.  **Add File:** Click the "Add file" button (usually near the top right of the file list) and select "Create new file".
3.  **Name Your File:** In the "Name your file..." box, type the filename for your project. Use a unique slug based on your project name, followed by `.json`. Use only lowercase letters, numbers, and hyphens (e.g., `my-awesome-app.json`). Place it in the root directory (don't add subfolders).
4.  **Add Content:**
    * Copy the contents of the `template.json` file.
    * Paste the template content into the large text editing box on the GitHub page.
    * **Edit the content**, replacing the placeholder values with your project's actual details. Ensure it is valid JSON (see **JSON Data Requirements** below).
5.  **Propose New File:** Scroll down below the editor. Add a short commit message (e.g., "Add showcase: My Awesome App") and optionally a description. Click the "Propose new file" button.
6.  **Open Pull Request:** GitHub will typically take you directly to a page to open a Pull Request. Review the details and click "Create pull request".

**Method 2: Using Git Locally (For more control or multiple changes)**

1.  **Fork this Repository:** Click the "Fork" button at the top right of this page to create your own copy.
2.  **Clone Your Fork:** Clone your forked repository to your local machine.
    ```bash
    git clone [https://github.com/YOUR_USERNAME/showcase.git](https://github.com/YOUR_USERNAME/showcase.git)
    cd showcase
    ```
3.  **Create a Branch:** Create a new branch for your submission. Use a descriptive name (e.g., `add-my-project-name`).
    ```bash
    git checkout -b add-my-project-name
    ```
4.  **Create & Edit JSON File:**
    * Copy the `template.json` file.
    * Rename the copied file to `your-project-slug.json` in the root directory (e.g., `my-awesome-app.json`).
    * Edit the file, filling in the JSON fields accurately with your project's details. Ensure it is valid JSON.
5.  **Commit Changes:** Stage and commit your new file with a clear commit message.
    ```bash
    git add your-project-slug.json
    git commit -m "feat: Add showcase submission for [Your Project Name]"
    ```
6.  **Push to Your Fork:** Push your new branch and commit to your forked repository on GitHub.
    ```bash
    git push origin add-my-project-name
    ```
7.  **Open a Pull Request:** Go back to the main `vibecoders/showcase` repository page on GitHub. You should see a prompt suggesting you create a Pull Request from the branch you just pushed. Click it, review your changes, add any relevant comments, and submit the Pull Request.
