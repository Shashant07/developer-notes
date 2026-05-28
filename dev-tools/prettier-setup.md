# 🚀 Prettier Setup Guide

Prettier automatically formats your code for consistent styling.

---

# 📦 Install Prettier

```bash
npm install -D prettier
````

---

# 📄 Create Prettier Config

Create file:

```txt
.prettierrc
```

Add:

```json id="74ix74"
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

# 🚫 Ignore Files

Create:

```txt id="d4chom"
.prettierignore
```

Add:

```txt id="59g4nk"
node_modules
dist
build
coverage
package-lock.json
```

---

# 📜 Add Script

Inside `package.json`:

```json id="z7z73q"
"scripts": {
  "format": "prettier --write ."
}
```

---

# ▶️ Run Formatter

```bash id="fyy9ae"
npm run format
```

---

# 💡 Benefits

* Clean code formatting
* Consistent styling
* Team standardization
* Faster development