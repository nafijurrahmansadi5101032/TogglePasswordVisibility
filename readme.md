# Password Visibility Toggle (Sign-In Form)

A lightweight, accessible, and responsive sign-in card built with vanilla HTML, modern CSS, and JavaScript. It features an interactive password visibility toggle that seamlessly switches between hidden and plain-text states using Bootstrap Icons.

---

## 🚀 Demo

- **Live Preview:** [Your Live Demo Link Here](https://nafijurrahmansadi5101032.github.io/TogglePasswordVisibility/)

---

## ✨ Features

- **Toggle Password Visibility:** Clickable eye icon to switch dynamically between masked (`password`) and readable (`text`) input modes.
- **Clean UI & Responsive Layout:** Fully centered responsive card layout styled with modern CSS.
- **Form Submission Handling:** Prevents page reloads on submit for seamless integration with AJAX / client-side authentication.
- **Pure Vanilla Stack:** Zero external JavaScript dependencies or bulky frameworks.
- **Accessible & Semantic HTML:** Structured with semantic tags (`<form>`, `<label>`, `<input>`, `<button>`).

---

## 📂 Project Structure

```plaintext
├── index.html       # Semantic HTML markup
├── styles.css       # Core styling, responsive design & absolute positioning
├── script.js        # DOM manipulation & visibility toggle logic
└── README.md        # Project documentation
```

---

## 🛠️ Built With

- **HTML5:** Semantic markup and accessibility standards.
- **CSS3:** Flexbox layout, CSS transitions, and responsive styling.
- **JavaScript (ES6):** Arrow functions, event listeners, and DOM attribute toggling.
- **[Bootstrap Icons](https://icons.getbootstrap.com/):** Vector icon library for the toggle eye button.

---

## ⚙️ How It Works

1. **State Detection & Switch:**
   When the user clicks the eye icon (`#togglePassword`), the script inspects the current `type` attribute of the `#password` field:
   ```javascript
   const type = password.getAttribute('type') === 'password' ? 'text' : 'password';
   password.setAttribute('type', type);
   ```
2. **Icon Feedback:**
   The icon's visual state updates by toggling the `bi-eye` class:
   ```javascript
   togglePassword.classList.toggle('bi-eye');
   ```
3. **Form Submission Interception:**
   Default submit behavior is prevented to allow custom verification logic:
   ```javascript
   form.addEventListener('submit', (e) => {
       e.preventDefault();
   });
   ```
