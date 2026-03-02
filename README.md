# YouTube Clone - Pure CSS

This is a responsive YouTube homepage clone built using **Pure CSS** (no JavaScript). It features a functional responsive grid, dark mode, interactive video previews, a playlist sidebar, and a login modal.

## 🚀 Features

### 1. Responsive Video Grid
- **Desktop:** 4 columns
- **Tablet:** 2-3 columns with collapsed sidebar
- **Mobile:** 1 column with bottom navigation

### 2. Dark Mode Toggle 🌙
- Implemented using the **Checkbox Hack**.
- Switches CSS variables for background, text, and border colors.
- Smooth transitions between themes.

### 3. Hover Video Preview 🎥
- **Pure CSS Animation:** Progress bar fills up on hover.
- **Transform Effects:** Thumbnails scale and tilt (3D effect).
- **Info Card:** Details slide up from the bottom on hover.

### 4. Playlist Sidebar 📂
- **Toggle Mechanism:** Checkbox hack controls visibility.
- **CSS Counters:** Automatically numbers playlist items.
- **Mini-Player:** Animated equalizer bars using CSS Keyframes.

### 5. Login Modal 👤
- **Target Selector:** Uses `:target` to show/hide the modal.
- **Floating Labels:** Form inputs animate labels on focus/valid state.
- **Tab Switching:** Radio button hack to switch between Sign In and Sign Up forms.

## 🛠️ CSS Hacks & Techniques Used

### The Checkbox Hack (`:checked`)
Used for global state management without JavaScript.
```css
/* Example: Dark Mode */
#theme-toggle:checked ~ .app-container {
    --bg-primary: #0f0f0f;
    /* ... other variables */
}
```

### The Target Hack (`:target`)
Used for the Modal popup.
```css
#login-modal:target {
    opacity: 1;
    visibility: visible;
}
```

### Sibling Selectors (`~` and `+`)
Used to control elements based on the state of previous elements (like checkboxes).

### CSS Variables
Used for easy theming and maintainability.

### CSS Grid & Flexbox
Used for the main layout and component structure.

## 📂 Project Structure
```
/
├── index.html      # Main structure
├── styles.css      # All styling and logic
├── assets/         # Asset folder
└── README.md       # Documentation
```

## 📸 How to Run
Simply open `index.html` in any modern web browser. No server or build process required.
