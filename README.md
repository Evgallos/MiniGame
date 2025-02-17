### 🕹 **MiniGame - C# Certification Challenge**  
**I created this project as a challenge and final project for my C# Certification - via Microsoft Learning.**  
An **interactive mini-game** where the player moves around collecting money, changing states based on the type of item collected.  

---

## 📌 **Project Overview**  
This game was built using **C#** and runs in the console. The player's goal is to collect different items while encountering random effects such as speed boosts or getting "sick."  

### 🎯 **Features**  
✔ Randomly generated collectible items 💰  
✔ Player movement controlled via **arrow keys** ⬆⬇⬅➡  
✔ Dynamic player states based on collected items  
✔ Resets when the console window resizes  
✔ Exit anytime with the **Escape** key  

---

## 🔧 **Technologies Used**  
- **C#** (Console Application)  
- **Randomization & Input Handling**  
- **Object Positioning & Console Rendering**  

---

## 📂 **Repository**  
🔗 [GitHub Repository](https://www.github.com/Evgallos/MiniGame)  

## 🌎 **Portfolio**  
📌 [Evgallos Portfolio - Live](https://www.evgallos.com)  

---

## ✨ **Key Code Snippet (YAML)**  
```yaml
name: MiniGame Build
on: [push, pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v3

      - name: Setup .NET
        uses: actions/setup-dotnet@v3
        with:
          dotnet-version: '7.0.x'

      - name: Restore Dependencies
        run: dotnet restore

      - name: Build the Project
        run: dotnet build --no-restore --configuration Release

      - name: Run Tests
        run: dotnet test --no-build --verbosity normal
```
This **GitHub Actions YAML** automates the build and test process, ensuring every commit is validated before deployment.  

---

🚀 **Hope you enjoy this project! Feel free to fork and experiment!** 💻
