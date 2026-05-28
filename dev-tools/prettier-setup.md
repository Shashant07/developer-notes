# 🚀 Prettier Setup for React + Vite + TypeScript

Prettier automatically formats code and maintains consistent styling across the project.

---

# 📦 Install Prettier

```bash
npm install -D prettier
````

---

# 📄 Create Prettier Config

Create:

```txt
.prettierrc
```

Add:

```json
{
  "semi": true,
  "singleQuote": true,
  "tabWidth": 2,
  "trailingComma": "all",
  "printWidth": 100,
  "arrowParens": "always"
}
```

---

# 🚫 Create Ignore File

Create:

```txt
.prettierignore
```

Add:

```txt
node_modules
dist
build
coverage
package-lock.json
```

---

# 📜 Add Format Scripts

Inside `package.json`:

```json
"scripts": {
  "format": "prettier --write .",
  "format:check": "prettier --check ."
}
```

---

# ▶️ Run Formatter

Format project:

```bash
npm run format
```

Check formatting:

```bash
npm run format:check
```

---

# 💡 Best Practices

* Use Prettier in all projects
* Enable VS Code format on save
* Keep formatting automatic
* Avoid manual formatting

---

# 🧩 Recommended VS Code Extensions

* Prettier - Code Formatter
* ESLint

---

# ⚙️ VS Code Settings

Create:

```txt
.vscode/settings.json
```

Add:

```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode"
}
```

---

# ✅ Benefits

* Consistent code style
* Cleaner pull requests
* Faster development
* Better team collaboration
