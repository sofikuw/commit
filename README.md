# commit

**commit** is a lightweight, zero-dependency client-side web tool that allows you to upload a `.zip` archive and commit its contents directly to any GitHub repository using the GitHub Git Data API.

## Features

- **Direct GitHub Integration**: Uses GitHub REST API (`/git/blobs`, `/git/trees`, `/git/commits`, `/git/refs/heads`) to push changes without needing local Git installation or command-line tools.
- **Root Directory Stripping**: Option to automatically detect and strip top-level archive wrapper directories (common when compressing folders on macOS/Windows).
- **Target Path Support**: Deploy files directly into a specific subfolder within your repository or to the root.
- **Force Push Support**: Option to overwrite commit history or merge with existing files in the target branch.
- **Minimalist Aesthetic**: Clean, modern dark-mode interface.

## How to Use

1. Open `index.html` in any web browser (or host it statically on GitHub Pages, Netlify, Vercel, etc.).
2. Enter your **GitHub Personal Access Token (PAT)** with repository permissions (`repo` scope).
3. Specify the target **Repository** (`username/repository`) and **Branch** (e.g., `main`).
4. (Optional) Provide a **Target Path** if you want files placed in a subfolder.
5. Enter a **Commit Message**.
6. Select your `.zip` archive file containing the files to upload.
7. Toggle **"Strip root directory from archive paths"** or **"Force push"** as needed.
8. Click **Deploy**.

## License

This project is released into the public domain under the [Unlicense](LICENSE).
