# 🗂️ GitHub Project Board: Integration Tracker

This board helps you track issues from reporting to resolution in a Kanban-style view.

## 🛠 Setup Steps

1. Go to your repository on GitHub
2. Click the `Projects` tab → Click **New Project**
3. Choose **Board** (or **Classic Project** if available)
4. Name your project: `Integration Issues Tracker`
5. Add the following columns:
   - 🆕 New
   - 🔍 Triaged
   - 🔧 In Progress
   - ✅ Resolved

## ⚙️ Add Automation Rules

For each column:
- Click the **⚙️ gear icon** in the column header
- Click **“Manage automation”**
- Set the automation based on labels:

| Column Name   | When this label is added           |
|---------------|------------------------------------|
| 🆕 New         | `status/new`                        |
| 🔍 Triaged     | `status/triaged`                    |
| 🔧 In Progress | `status/in-progress` *(optional)*   |
| ✅ Resolved    | `status/resolved`                   |

> Make sure these labels exist in your repo (see `labels.yml`).

## 📌 Example Workflow

1. User creates an issue via template
2. Label `status/new` is applied automatically
3. Issue appears in the **New** column
4. Once triaged, you change the label to `status/triaged` and it moves to **Triaged**
5. Development starts: change label to `status/in-progress`
6. When resolved: apply `status/resolved`

## ✅ Tip

You can manually drag issues between columns too!

---

Happy tracking! 📊
