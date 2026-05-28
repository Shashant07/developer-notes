# 🚀 Husky + ESLint + lint-staged Setup

Professional Git hooks setup for React + Vite + TypeScript projects.

This setup automatically:
- Runs ESLint
- Formats code with Prettier
- Checks staged files only
- Prevents bad commits

---

# 📦 Install Required Packages

```bash
npm install -D husky lint-staged prettier
````

---

# 📜 Add Scripts

Inside `package.json`:

```json
"scripts": {
  "prepare": "husky",
  "lint": "eslint .",
  "lint:fix": "eslint . --fix",
  "format": "prettier --write ."
}
```

---

# ⚙️ Configure lint-staged

Inside `package.json`:

```json
"lint-staged": {
  "*.{js,jsx,ts,tsx}": [
    "eslint --fix",
    "prettier --write"
  ],
  "*.{json,css,scss,md}": [
    "prettier --write"
  ]
}
```

---

# 🐶 Initialize Husky

```bash
npx husky init
```

This creates:

```txt
.husky/
```

---

# 🔗 Configure Pre-Commit Hook

Open:

```txt
.husky/pre-commit
```

Replace content with:

```bash
npx lint-staged
```

---

# 🚀 Test Setup

Stage files:

```bash
git add .
```

Commit changes:

```bash
git commit -m "chore: setup husky and lint-staged"
```

Husky will now:

* Run ESLint
* Run Prettier
* Check staged files only

---

# 💡 Best Practices

* Run checks before every commit
* Keep hooks fast
* Lint only staged files
* Use consistent formatting
* Never bypass hooks unnecessarily

---

# 📂 Final Recommended Structure

```txt
project/
│
├── .husky/
├── .prettierrc
├── .prettierignore
├── eslint.config.js
├── package.json
└── src/
```

---

# ✅ Benefits

* Cleaner commits
* Better code quality
* Automated formatting
* Prevents broken code
* Professional workflow
