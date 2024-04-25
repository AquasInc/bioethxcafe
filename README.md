# Astro Dev set up


## 🧑‍🚀 Set up git

Download Git instructions for [windows](https://git-scm.com/download/win)

```sh
# Install git via package manager e.g. apt
sudo apt install git

# Add your contact details to see who authored commits to history
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"

# Set default branch to main to correspond to github's default
git config --global init.defaultBranch main

# Clone project locally with git
git clone https://github.com/AquasInc/bioethxcafe.git
```
Download your standard text editor [vscode](https://code.visualstudio.com/)

```sh
# Set up remote github repository so you can push your local changes to upstream
git remote add origin https://github.com/AquasInc/bioethxcafe.git

# Make small edits to the cloned project and add the edited files that you want to commit to version control 
git add <file> 

# commit those changes to version control with a minimal message detailing your change 
git commit -m "<message>" 

# Check for any upstream changes to the project before pushing your local changes to upstream 
git fetch 

# When you are ready to push your changes to production
git push
```

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
