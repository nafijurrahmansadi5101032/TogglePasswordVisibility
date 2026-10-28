Password Visibility Toggle (Sign-In Form)

A lightweight, accessible, and responsive sign-in card built with vanilla HTML, modern CSS, and JavaScript. It features an interactive password visibility toggle that seamlessly switches between hidden and plain-text states using Bootstrap Icons.

🚀 Demo

Live Preview: Your Live Demo Link Here

✨ Features

Toggle Password Visibility: Clickable eye icon to switch dynamically between masked (password) and readable (text) input modes.

Clean UI & Responsive Layout: Fully centered responsive card layout styled with modern CSS.

Form Submission Handling: Prevents page reloads on submit for seamless integration with AJAX / client-side authentication.

Pure Vanilla Stack: Zero external JavaScript dependencies or bulky frameworks.

Accessible & Semantic HTML: Structured with semantic tags (<form>, <label>, <input>, <button>).

📂 Project Structure

├── index.html       # Semantic HTML markup
├── styles.css       # Core styling, responsive design & absolute positioning
├── script.js        # DOM manipulation & visibility toggle logic
└── README.md        # Project documentation


🛠️ Built With

HTML5: Semantic markup and accessibility standards.

CSS3: Flexbox layout, CSS transitions, and responsive styling.

JavaScript (ES6): Arrow functions, event listeners, and DOM attribute toggling.

Bootstrap Icons: Vector icon library for the toggle eye button.

⚙️ How It Works

State Detection & Switch:
When the user clicks the eye icon (#togglePassword), the script inspects the current type attribute of the #password field:

const type = password.getAttribute('type') === 'password' ? 'text' : 'password';
password.setAttribute('type', type);


Icon Feedback:
The icon's visual state updates by toggling the bi-eye class:

togglePassword.classList.toggle('bi-eye');


Form Submission Interception:
Default submit behavior is prevented to allow custom verification logic:

form.addEventListener('submit', (e) => {
    e.preventDefault();
});


🚀 Getting Started

Prerequisites

All you need is a modern web browser (e.g., Chrome, Edge, Firefox, Safari).

Installation & Local Setup

Clone the repository:

git clone https://github.com/your-username/password-toggle-form.git


Navigate to the project directory:

cd password-toggle-form


Open the project:

Double-click index.html to open it directly in your browser, or

Use VS Code with the Live Server extension.

🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📝 License

Distributed under the MIT License.