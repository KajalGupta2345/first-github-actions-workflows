# 🚀 GitHub Actions Demo

## 📌 Project Overview

Is project ka purpose **GitHub Actions** ko samajhna aur use karna hai. GitHub Actions ek automation tool hai jo repetitive tasks ko automatically perform karta hai.

Jaise hi developer GitHub par code push karta hai, GitHub Actions automatically build, test aur deploy jaise tasks perform kar sakta hai.

---

## 🤔 GitHub Actions Kya Hai?

GitHub Actions GitHub ka ek feature hai jo workflows ko automate karta hai.

Simple words me:

> "Aap code likho aur GitHub ko bata do ki code push hone ke baad kya karna hai. Baaki kaam GitHub Actions automatically kar dega."

Example:

* Code Test Karna
* Project Build Karna
* Website Deploy Karna
* Notifications Send Karna

---

## 🎯 GitHub Actions Kyu Use Karte Hain?

Agar hum manually kaam karein to har baar:

1. Code Push Karna
2. Dependencies Install Karna
3. Tests Run Karna
4. Build Banana
5. Deploy Karna

Ye sab manually karna padega.

GitHub Actions use karne par:

```text
Code Push
   ↓
GitHub Actions Start
   ↓
Testing
   ↓
Build
   ↓
Deploy
```

Sab automatically ho jata hai.

---

## ⚙️ GitHub Actions Kaise Kaam Karta Hai?

GitHub repository ke andar ek folder hota hai:

```text
.github/workflows/
```

Is folder ke andar YAML file hoti hai.

Example:

```text
.github/workflows/deploy.yml
```

Ye file GitHub ko instructions deti hai ki kya kaam karna hai aur kab karna hai.

---

## 🧩 Important Terms

### 1. Workflow

Workflow ek complete automation process hota hai.

Example:

```text
Install Dependencies
↓
Run Tests
↓
Build Project
↓
Deploy Project
```

Ye poora workflow hai.

---

### 2. Event

Event batata hai workflow kab start hoga.

Example:

```yaml
on:
  push
```

Matlab code push hote hi workflow run hoga.

---

### 3. Job

Workflow ke andar jo major task hota hai use Job kehte hain.

Example:

```yaml
jobs:
  build:
```

---

### 4. Step

Job ke andar chhote-chhote commands ko Steps kehte hain.

Example:

```yaml
steps:
  - run: npm install
  - run: npm test
```

---

## 💻 Sample Workflow

```yaml
name: Build Project

on:
  push:
    branches:
      - main

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - uses: actions/setup-node@v4
        with:
          node-version: 20

      - run: npm install

      - run: npm run build
```

---

## 🚀 Real-Life Example

Maan lo tumhari React Portfolio Website hai.

Normal Process:

```text
Code Change
↓
Build
↓
Deploy
↓
Check Website
```

Sab manually.

GitHub Actions Ke Saath:

```text
Code Push
↓
Automatic Build
↓
Automatic Deploy
↓
Website Updated
```

Koi manual work nahi.

---

## ✨ Advantages

✅ Time Bachata Hai

✅ Manual Work Kam Karta Hai

✅ Automatic Testing

✅ Automatic Deployment

✅ Better Code Quality

✅ Faster Development Process

✅ Easy CI/CD Setup

---

## 🔄 CI/CD Kya Hai?

### Continuous Integration (CI)

Continuous Integration ka matlab hai ki jab bhi developer code me changes karke GitHub par push karta hai, to project automatically check hota hai.

CI me generally ye kaam hote hain:

* Code Build Karna
* Tests Run Karna
* Errors Check Karna
* Code Quality Verify Karna

Example:

```text
Developer Code Push Karta Hai
            ↓
GitHub Actions Trigger Hota Hai
            ↓
Tests Run Hote Hain
            ↓
Build Successfully Complete Hota Hai
```

Isse bugs jaldi pakde jate hain aur code quality maintain rehti hai.

---

### Continuous Deployment (CD)

Continuous Deployment ka matlab hai ki agar build aur tests successfully pass ho jayein to application automatically deploy ho jati hai.

Example:

```text
Code Push
    ↓
Tests Pass
    ↓
Build Success
    ↓
Automatic Deployment
```

Developer ko manually deployment karne ki zarurat nahi padti.

---

## 🚀 GitHub Actions Aur CI/CD

GitHub Actions CI/CD pipeline create karne ke liye use kiya jata hai.

Example Workflow:

```text
Code Push
    ↓
GitHub Actions Start
    ↓
Install Dependencies
    ↓
Run Tests
    ↓
Build Project
    ↓
Deploy Project
```

Yahan:

* **CI (Continuous Integration)** = Install Dependencies + Testing + Build
* **CD (Continuous Deployment)** = Automatic Deployment

---

## 🎯 CI/CD Ke Benefits

✅ Bugs Jaldi Detect Hote Hain

✅ Code Quality Improve Hoti Hai

✅ Faster Development

✅ Automated Testing

✅ Automated Deployment

✅ Human Errors Kam Hote Hain

✅ Time Aur Effort Dono Bachate Hain

---




---

