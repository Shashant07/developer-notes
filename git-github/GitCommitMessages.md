# 🚀 Best Practices for Git Commit Messages

Clean and professional commit messages help maintain better project history and collaboration.

---

# 📌 Recommended Commit Format

```bash
type: short description
````

Example:

```bash id="59z4s9"
feat: add login authentication
fix: resolve navbar issue
docs: add README documentation
```

---

# 🛠️ Common Commit Types

| Type     | Purpose            |
| -------- | ------------------ |
| feat     | New feature        |
| fix      | Bug fix            |
| docs     | Documentation      |
| style    | UI/CSS formatting  |
| refactor | Code improvement   |
| test     | Test updates       |
| chore    | Config/maintenance |

---

# ✅ Best Practices

## 1. Keep Message Short

```bash id="rctvzs"
feat: add dark mode
```

---

## 2. Use Present Tense

✅ Good:

```bash id="i3wb3i"
fix: resolve API issue
```

❌ Bad:

```bash id="r98fd9"
fixed API issue
```

---

## 3. Be Specific

✅ Good:

```bash id="utn2ye"
fix: correct mobile navbar overflow
```

❌ Bad:

```bash id="jlwm2m"
fix: bug fixes
```

---

## 4. One Commit = One Purpose

✅ Good:

```bash id="k4k2l4"
feat: add JWT authentication
```

Separate UI changes into another commit.

---

# 🚀 Git Workflow

```bash id="p9evj0"
git status
git add .
git commit -m "feat: add dashboard page"
git push
```

---

# 💡 Recommended Commit Examples

```bash id="jjab7h"
feat: add authentication flow
fix: resolve TypeScript errors
docs: add husky setup guide
style: improve dashboard spacing
refactor: optimize API structure
```

---

# ❌ Avoid These Messages

```bash id="n0wpft"
update
done
changes
final
working
test
```

---

# 🎯 Goal

Write clean, meaningful, and professional commit messages for better collaboration and project maintenance.
