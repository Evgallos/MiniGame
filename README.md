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

## ✨🍽️ Spawning Random Food in the Game
The following function randomly places food at a new location within the console window. Each food type has a unique effect on the player when collected.

```yaml
// Displays random food at a random location
void ShowFood()
{
    // Update food to a random index
    food = random.Next(0, foods.Length);

    // Update food position to a random location
    foodX = random.Next(0, width - player.Length);
    foodY = random.Next(0, height - 1);

    // Display the food at the location
    SetCursorPosition(foodX, foodY);
    Write(foods[food]);
}
```
This function ensures that food appears at different positions each time, making the game dynamic and engaging! 🎮🔥

---

🚀 **Hope you enjoy this project! Feel free to fork and experiment!** 💻
