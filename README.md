# ✨ Vibe Check Machine

<div align="center">

![License: MIT](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

A fun, interactive quiz application that determines your personality vibe in 5 hilarious questions. Built with vanilla JavaScript, HTML5, and CSS3.

[🚀 Live Demo](#live-demo) • [📋 Features](#features) • [🛠️ Tech Stack](#tech-stack) • [📦 Installation](#installation)

</div>

---

## 🎯 Overview

**Vibe Check Machine** is a modern, interactive personality quiz that analyzes your answers across 5 quirky questions and assigns you one of four personality archetypes. With smooth animations, a beautiful gradient UI, and responsive design, it's perfect for entertainment or as a portfolio project showcase.

The quiz uses a point-based scoring system (0-15 points total) to categorize users into:
- 🛋️ **The Cozy Sloth** (0-3 points)
- 🌿 **The Balanced Sage** (4-6 points)  
- ⚡ **The Chaotic Star** (7-9 points)
- 🚀 **The Galaxy Brain** (10-15 points)

---

## ✨ Features

✅ **Interactive Quiz Interface**
- 5 personality-defining questions
- A, B, C, D answer options with point values
- Smooth transitions between questions

✅ **Real-time Progress Tracking**
- Visual progress bar showing quiz completion
- Question counter (e.g., "Question 2 of 5")
- Instant feedback on selections

✅ **Beautiful UI/UX Design**
- Gradient backgrounds with vibrant colors
- Animated blob elements for visual appeal
- Emoji-based personality results
- Fully responsive mobile-first design

✅ **Result Calculation**
- Dynamic scoring system
- Personalized vibe descriptions
- Easy restart functionality

✅ **Code Quality**
- Clean, well-documented JavaScript
- Professional CSS with CSS variables
- Semantic HTML5 structure
- JSDoc comments for functions

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| **HTML5** | Semantic markup & structure |
| **CSS3** | Modern styling, animations, gradients |
| **JavaScript (ES6+)** | Quiz logic, DOM manipulation, scoring |
| **Google Fonts** | Typography (Fredoka, Nunito) |

**No frameworks or dependencies required** — Pure vanilla implementation!

---

## 📦 Installation

### Option 1: Clone the Repository
```bash
# Clone the repo
git clone https://github.com/mianhasssan/vibe-check-machine.git

# Navigate to the directory
cd vibe-check-machine

# Open in your browser
open index.html
# Or simply drag index.html into your browser
```

### Option 2: Download as ZIP
1. Click **Code** → **Download ZIP**
2. Extract the files
3. Open `index.html` in your browser

### Option 3: Use Live Server (Recommended)
```bash
# Install Live Server globally (if not already installed)
npm install -g live-server

# Navigate to project directory
cd vibe-check-machine

# Start live server
live-server
```

---

## 🚀 Usage

1. **Start the Quiz**: Click "Let's Go! 🚀" on the home screen
2. **Answer Questions**: Select one of four options (A, B, C, or D) for each question
3. **View Results**: After all 5 questions, see your personality vibe with emoji and description
4. **Try Again**: Click "Try Again 🔄" to restart with fresh scoring

### Questions Covered:
1. 🌅 Saturday morning habits
2. 📱 Phone battery anxiety levels
3. 🍕 Problem-solving approach
4. 🎶 Study environment preferences
5. 🌈 Weekend trip ideal vibe

---

## 📁 Project Structure

```
vibe-check-machine/
├── index.html          # Main HTML file
├── index.js            # Core quiz logic
├── index.css           # Styling & animations
├── README.md           # This file
├── .gitignore          # Git ignore rules
└── LICENSE             # MIT License
```

### File Descriptions

**index.html**
- Semantic HTML5 structure
- Three main screens: Start, Quiz, Results
- Links to CSS and JavaScript files
- Meta tags for responsive design

**index.js**
- `startQuiz()` - Initializes the quiz
- `showQuestion()` - Displays current question and choices
- `selectChoice()` - Handles answer selection and scoring
- `showResult()` - Displays final personality vibe
- `computeVibe()` - Scoring logic and vibe determination
- `switchScreen()` - Manages screen transitions

**index.css**
- CSS variables for theming and maintainability
- Mobile-first responsive design
- Gradient animations and blob animations
- Smooth transitions and hover effects

---

## 🎨 Customization

### Change Personality Results
Edit the `computeVibe()` function in `index.js`:

```javascript
function computeVibe(totalScore) {
    if (totalScore <= 3) {
        return {
            emoji: "🛋️",
            title: "Your Custom Title",
            desc: "Your custom description here"
        };
    }
    // ... more conditions
}
```

### Modify Questions
Update the `questions` array in `index.js`:

```javascript
const questions = [
    {
        text: "Your question here?",
        choices: [
            { label: "Option 1", points: 0 },
            { label: "Option 2", points: 1 },
            { label: "Option 3", points: 2 },
            { label: "Option 4", points: 3 },
        ]
    },
    // ... more questions
];
```

### Change Color Scheme
Modify CSS variables in `index.css`:

```css
:root {
    --primary-color: #667eea;      /* Change to your color */
    --secondary-color: #764ba2;    /* Change to your color */
    --accent-color: #f093fb;       /* Change to your color */
    /* ... more variables */
}
```

---

## 🔄 How Scoring Works

Each answer choice has a point value (0-3):
- **0 points**: Relaxed/Minimalist approach
- **1 point**: Moderate/Balanced approach  
- **2 points**: Proactive/Engaged approach
- **3 points**: Extreme/Adventurous approach

**Total Score Ranges:**

| Score Range | Personality Type |
|-----------|-----------------|
| 0-3 | 🛋️ Cozy Sloth |
| 4-6 | 🌿 Balanced Sage |
| 7-9 | ⚡ Chaotic Star |
| 10-15 | 🚀 Galaxy Brain |

---

## 🌐 Browser Compatibility

| Browser | Status |
|---------|--------|
| Chrome | ✅ Full Support |
| Firefox | ✅ Full Support |
| Safari | ✅ Full Support |
| Edge | ✅ Full Support |
| IE 11 | ⚠️ Partial (no CSS variables) |

---

## 📱 Responsive Design

The application is fully responsive and optimized for:
- **Desktop**: Full UI with blob animations
- **Tablet**: Optimized spacing and touch targets
- **Mobile**: Simplified layout, no blob animations for performance

---

## 🚀 Performance Optimizations

✅ **Lightweight**: No dependencies, minimal file sizes
- `index.html`: ~2KB
- `index.js`: ~4KB  
- `index.css`: ~8KB

✅ **Fast Loading**: Google Fonts preconnected
✅ **Smooth Animations**: GPU-accelerated transforms
✅ **Minimal Reflows**: Efficient DOM updates

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. **Fork the repository**
   ```bash
   git clone https://github.com/mianhasssan/vibe-check-machine.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Commit with clear messages
   - Follow the existing code style

4. **Push and submit a Pull Request**
   ```bash
   git push origin feature/your-feature-name
   ```

### Ideas for Contribution:
- 🎨 New color themes/skins
- 📝 Additional questions/personalities
- 🌍 Internationalization (i18n)
- 🎯 Improved accessibility (a11y)
- 📊 Result sharing features
- 🧪 Unit tests

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

You're free to use, modify, and distribute this project for personal and commercial purposes.

---

## 👨‍💻 Author

**Mian Muhammad Hassan**

- 🔗 [GitHub](https://github.com/mianhasssan)
- 🔗 [LinkedIn](https://linkedin.com/in/mianmuhammadhassan322)
- 📧 [Email](mailto://mmh427726@gmail.com)

---

## 🎓 Learning Resources

This project demonstrates:
- ✅ Vanilla JavaScript (no frameworks)
- ✅ DOM manipulation & event handling
- ✅ CSS animations & gradients
- ✅ Responsive design principles
- ✅ Clean code practices & documentation
- ✅ Git version control

Great for beginners learning **frontend development**!

---

## 🐛 Bug Reports & Feature Requests

Found a bug or have a feature idea? Please open an **issue** on GitHub:

[Report an Issue](https://github.com/mianhasssan/vibe-check-machine/issues)

---

## 🌟 Show Your Support

If you find this project useful or fun, please consider:
- ⭐ Starring the repository
- 🔗 Sharing it with others
- 💬 Leaving feedback or suggestions
- 🤝 Contributing improvements

---

<div align="center">

### Made with ❤️ by [Mian Muhammad Hassan](https://github.com/mianhasssan)

**Happy vibe checking! 🚀✨**

</div>
