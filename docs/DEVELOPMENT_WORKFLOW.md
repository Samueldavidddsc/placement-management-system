# SDC Frontend: Simple Contributor Guide 🚀

> **Welcome to the SDC Frontend Team!**  
> We build the DKTE Placement Portal together. Here is the super-simple guide on how we work so no one feels lost or overwhelmed.

---

## 🛑 The 3 Simple Rules

1. **No new `.css` files**  
   Use Tailwind CSS classes (like `bg-blue-600`, `p-4`, `rounded-lg`). It keeps our code clean and fast.
2. **No fake/mock data**  
   The backend team already built real APIs for us (Student data, drives, companies). We hook our screens to their real data.
3. **Pick 1 task at a time**  
   Don't try to build an entire page alone. Pick one small task from GitHub, finish it, and submit it.

---

## 🔄 The 4 Steps to Build Something

Whenever you want to build or fix something, follow these 4 steps:

### 1. Pick a Task on GitHub
* Go to the **GitHub Issues** tab.
* Find a task marked with `good-first-issue` or `P0`.
* Comment on the issue: *"I want to work on this!"*

### 2. Make a New Branch
Open your terminal and type:
```bash
# Get the latest code
git checkout main
git pull

# Create your branch (give it a simple name)
git checkout -b feat/add-button
```

### 3. Build & Test It
* Start your local server:
  ```bash
  cd frontend
  npm run dev
  ```
* Open `http://localhost:3000` in your browser and write your code.
* Before saving your work, make sure it builds without errors:
  ```bash
  npm run build
  ```

### 4. Send Your Code (Pull Request)
* Push your code to GitHub:
  ```bash
  git add .
  git commit -m "Add reusable Button component"
  git push origin feat/add-button
  ```
* Go to GitHub, click **Compare & pull request**.
* Add a screenshot of your work.
* Tag `@Farooq` for review! Once approved, your code gets merged into the real app! 🎉

---

## 🤝 Need Help?
* **Never stay stuck alone!** If you don't know how to style something or how an API works, ask in our WhatsApp/Discord group.
* You can also pair up with a teammate and build a task together!
