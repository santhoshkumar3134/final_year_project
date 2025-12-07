# 🛠️ Git Workflow Guide for Team Collaboration
> 🎯 Follow this workflow to avoid conflicts and maintain clean development flow.

---

## 🟦 1. Clone the Project (First-Time Setup)
```bash
git clone <repository-url>
cd project-folder-name
```

---

## 🟩 2. Create Your Own Branch (Recommended)
```bash
git checkout -b your-branch-name
```
Examples:
```bash
git checkout -b frontend-santhosh
git checkout -b backend-sharan
git checkout -b ml-rakesh
```

---

## 🟨 3. Always Pull Before Starting Work
```bash
git pull origin main
```
If you're on another branch:
```bash
git pull origin your-branch-name
```

---

## 🟪 4. Add Your Changes
Add all files:
```bash
git add .
```
Add a specific file:
```bash
git add filename.py
```

---

## 🟧 5. Commit Your Changes
```bash
git commit -m "Meaningful description of your update"
```
Good examples:
- Updated UI components  
- Added ML model  
- Fixed backend error  

---

## 🟥 6. Push Your Changes
```bash
git push origin your-branch-name
```

---

## 🔵 7. Create a Pull Request (PR)
1. Go to GitHub → Pull Requests  
2. Click **New Pull Request**  
3. Choose your branch → compare with `main`  
4. Add description  
5. Submit PR  
6. Team lead reviews & merges  

---

## 🔶 8. Handling Merge Conflicts
If you see something like this:
```txt
<<<<<<< HEAD
Your code
=======
Other teammate’s code
>>>>>>> main
```
Fix manually, then run:
```bash
git add .
git commit -m "Resolved merge conflict"
git push origin your-branch-name
```

---

## 🟫 9. Update Your Branch After Merge
Switch to main:
```bash
git checkout main
```
Pull latest:
```bash
git pull origin main
```
Merge main into your branch:
```bash
git checkout your-branch-name
git merge main
```

---

## 🧩 10. Project Folder Structure
```
LoanLite/
│── frontend/
│── backend/
│── ml-model/
│── docs/
│── README.md
│── GIT_WORKFLOW_GUIDE.md
```

---

## ⭐ 11. Team Collaboration Rules
- Always pull before starting work  
- Never push directly to main  
- Use meaningful commit messages  
- Communicate before major modifications  
- Each feature must be on its own branch  

---

## ⚡ 12. Quick Command Reference
```bash
git clone <URL>
git pull origin main
git checkout -b new-branch
git add .
git commit -m "Message"
git push origin new-branch
```

---

# 🚀 Teamwork = Clean Code + Zero Conflicts
> Keep following this workflow for smooth, conflict-free development.
