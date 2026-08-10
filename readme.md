# A11y Fix It

This project includes a set of components that are inaccessible. The goal is to fix the code so they are accessible and to fix any other accessibility issues found on the page.

You will work locally on your own copy, but you can also <a href="https://uw-ats.github.io/a11y-fixit/">view the exercise page here</a>.

## Set up

Clone or download the zip drive for the project via the Code selection box. Set up to work locally. The project uses JavaScript modules so you will need a local web server to run in the browser. If you are using Visual Studio Code for your IDE, the Live Preview extension by Microsoft is a good option.

## For contributors: Code Formatting Setup (Prettier + VS Code)

This project uses Prettier for consistent formatting across HTML, CSS, JavaScript, JSONC, and Markdown. Please set up the following if contributing to the project

### 1. Install the required VS Code extension

Install the extension:

- Prettier - Code formatter
- Publisher: Prettier
- Extension ID: esbenp.prettier-vscode

### 2. In your VS Code workspace, add these settings for formatter routing

(Note: there is not a common VS Code workspace added to the repo.)

Create workspace settings and add:

```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[markdown]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```

### 3. Prettier config at the project root

The prettier.config has been added to the project root with these settings:

```json
{
  "printWidth": 80,
  "tabWidth": 2,
  "useTabs": false,
  "semi": true,
  "singleQuote": false,
  "trailingComma": "all",
  "bracketSpacing": true,
  "arrowParens": "always",
  "endOfLine": "lf",
  "proseWrap": "preserve"
}
```

### 5. Verify it is working

1. Open any HTML, CSS, JavaScript, JSONC, or Markdown file.
2. Save the file.
3. Formatting should run automatically.
4. If needed, run Format Document With... once and pick Prettier for that language.

### 6. Troubleshooting

- Confirm Prettier extension is installed and enabled.
- Confirm Format on Save is enabled.
- Check for any language-specific user setting forcing another formatter.
- Open the Output panel and select Prettier to inspect formatter logs.
