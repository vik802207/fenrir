# Fenrir Security Technical Assignment

## 📌 Objective

This is a customized build of [Visual Studio Code](https://github.com/microsoft/vscode) with the open-source extension [Wingman AI](https://github.com/RussellCanfield/wingman-ai) **baked in as a native feature**.

### ✅ Achievements

- Wingman AI loads automatically on first launch
- Hidden from the Extensions panel / Marketplace
- Cannot be removed or disabled via normal UI
- All standard VS Code functionality remains intact

---

## 🧩 Key Modifications

### 📁 `extensions/wingman-ai/`
The Wingman AI `.vsix` was extracted and added to this path.

- `package.json` inside Wingman AI was modified to include:

```json
"builtIn": true
```
## 🛠️ VS Code Core Edits
build/builtInExtensions.json updated to register Wingman as a default extension

product.json modified to suppress Marketplace visibility (e.g., disable gallery extensions)
## 🛠️ Build Instructions
``` bash
1. Clone the Repository
git clone https://github.com/vik802207/Fenrir-Security-Assignment.git
cd Fenrir-Security-Assignment
2. Install Dependencies
npm install
3. Build VS Code
./scripts/code.sh           # For Linux/macOS
# or
.\scripts\code.bat          # For Windows
➡️ This will generate a portable VS Code build inside the .build directory.
```
---

## 📄 License

This project is developed solely for **Fenrir Security Private Limited** as part of a confidential technical screening assignment.  
All code, documentation, and media included are the **exclusive property of Fenrir Security**.

> 🔒 Do **not** distribute, share, or reuse any portion of this project outside the authorized evaluation process.

---

## 📬 Contact

**Candidate Name**: Vikash Gupta  
**Email**: vik802207@gmail.com  
**GitHub**: [@vik802207](https://github.com/vik802207)  
**Submission Date**: 18 June 2025  
**Assignment**: Custom VS Code with Wingman AI Integration

---


