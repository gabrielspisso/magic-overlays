# Tauri React Vite App

This project is a Tauri application built with React and Vite. It serves as a desktop application that leverages web technologies to create a native experience.

## Project Structure

- `src/`: Contains the main React application code.
  - `App.tsx`: The main React component that serves as the entry point for the application.
  - `main.tsx`: Responsible for rendering the React application into the DOM and integrating it with Tauri.
  - `vite-env.d.ts`: Provides TypeScript definitions for Vite-specific features.

- `public/`: Contains static assets.
  - `index.html`: The main HTML file that serves as the template for the application.

- `src-tauri/`: Contains the Tauri backend code.
  - `src/main.rs`: The main Rust code for the Tauri backend.
  - `Cargo.toml`: Configuration file for the Rust project.
  - `tauri.conf.json`: Configuration settings for the Tauri application.

- `package.json`: Configuration file for npm, listing dependencies and scripts.

- `tsconfig.json`: Configuration file for TypeScript, specifying compiler options.

- `vite.config.ts`: Configuration file for Vite, defining build and development settings.

- `.gitignore`: Specifies which files and directories should be ignored by Git.

## Getting Started

### Prerequisites

- Ensure you have [Node.js](https://nodejs.org/) installed.
- Install [Rust](https://www.rust-lang.org/tools/install) if you haven't already.

### Install NVM and Node.js

1. Install NVM:
   ```
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
   ```

2. Load NVM (you may need to restart your terminal or run the following command):
   ```
   export NVM_DIR="$HOME/.nvm"
   [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
   ```

3. Install a specific version of Node.js (e.g., version 16):
   ```
   nvm install 16
   ```

4. Use the installed version:
   ```
   nvm use 16
   ```

### Install Dependencies

Run the following command to install the project dependencies:
```
npm install
```

### Start the Tauri App

To start the Tauri development server, run:
```
npm run tauri dev
```

This will launch the Tauri application in development mode. You can make changes to your React components, and the app will automatically reload to reflect those changes.

### Use on WSL
Read [this guide](https://x410.dev/cookbook/wsl/using-x410-with-wsl2/).