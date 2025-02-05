# WEB TASK 1


# 🌟 **Todo List Web Application** 🌟

Welcome to the **Todo List Web Application**! This project is a sleek, user-friendly, and feature-packed task management tool built using **HTML**, **CSS**, and **JavaScript**. Whether you're a productivity enthusiast or just someone looking to organize your daily tasks, this app has got you covered. With a **theme switcher**, **local storage support**, and a responsive design, it’s the perfect companion for managing your todos efficiently.

---

## 📌 **Table of Contents**
1. [Introduction](#-introduction)
2. [Features](#-features)
3. [Requirements](#-requirements)
4. [Installation](#-installation)
5. [Usage](#-usage)
6. [Code Walkthrough](#-code-walkthrough)

---

## 🚀 **Introduction**

The **Todo List Web Application** is a lightweight yet powerful tool designed to help you manage your tasks with ease. It allows you to **add**, **edit**, **delete**, and **organize** your todos seamlessly. The app also includes a **theme switcher** to personalize your experience and uses **local storage** to save your todos and theme preferences, ensuring your data is always safe and accessible.

---

## ✨ **Features**

- **Add Todos**: Quickly add new tasks to your list.
- **Edit Todos**: Update existing tasks with ease.
- **Delete Todos**: Remove tasks you no longer need.
- **Delete All Todos**: Clear your entire list with a single click.
- **Theme Switcher**: Choose from multiple themes to customize the app's appearance.
- **Local Storage**: Todos and themes are saved in your browser, so your data persists even after closing the app.
- **Responsive Design**: Works flawlessly on both desktop and mobile devices.

---

## 📋 **Requirements**

- A modern web browser (Chrome, Firefox, Safari, Edge, etc.).
- No additional installations are required—just open the app and start using it!

---

## 🛠️ **Installation**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/todo-list.git
   cd todo-list
   ```

2. **Open the Application**:
   - Open the `index.html` file in your browser:
     ```bash
     open index.html
     ```

---

## 🖥️ **Usage**

1. **Add a Todo**:
   - Type your task in the input field and press `Enter` or click the `+` button.

2. **Edit a Todo**:
   - Click the edit button (pencil icon) next to a task, update the task, and click the checkmark button to save.

3. **Delete a Todo**:
   - Click the delete button (trash icon) next to a task.

4. **Delete All Todos**:
   - Click the "Delete All" button to clear the entire list.

5. **Change Theme**:
   - Click the palette icon in the top-right corner and select a theme from the dropdown.

---

## 🧑‍💻 **Code Walkthrough**

### **HTML Structure**
The `index.html` file defines the structure of the Todo List, including the input field, buttons, and task list.

```html
<div class="container">
    <header>
        <h1>Todo List</h1>
        <div class="input-section">
            <input type="text" placeholder="Add a todo . . ." />
            <button class="btn btn-secondary add-task-button">
                <i class="bx bx-plus bx-sm"></i>
            </button>
        </div>
    </header>
    <ul class="todos-list"></ul>
</div>
```

### **CSS Styling**
The `style.css` file provides the visual styling for the app, including layout, colors, and animations.

```css
.container {
    background: rgba(255, 255, 255, 0.15);
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.3);
    backdrop-filter: blur(3px);
    border-radius: 10px;
    padding: 20px;
}
```

### **JavaScript Functionality**
The `main.js` file handles the logic for adding, editing, deleting, and managing todos.

```javascript
function addToDo(task_input) {
    let task = {
        id: getRandomId(),
        task: task_input.value,
        completed: false
    }
    todos.push(task);
}
```

### **Theme Switcher**
The `theme_switcher.js` file allows users to switch between themes and saves the selected theme in local storage.

```javascript
themes.forEach(theme => {
    theme.addEventListener('click', () => {
        const theme_name = theme.getAttribute('theme');
        html.setAttribute('data-theme', theme_name);
        saveTheme(theme_name);
    });
});
```

---



# WEB TASK 2


# 🎓 **Student Registration Form** 🎓

Welcome to the **Student Registration Form** project! This is a sleek, user-friendly, and responsive web application designed to collect and display student information effortlessly. Whether you're managing student data for a school, college, or any educational institution, this form simplifies the process with its intuitive design and dynamic functionality.

---

## 📌 **Table of Contents**
1. [Project Overview](#-project-overview)
2. [Features](#-features)
3. [How It Works](#-how-it-works)
4. [Technologies Used](#-technologies-used)
5. [Installation](#-installation)
6. [Usage](#-usage)

---

## 🚀 **Project Overview**

The **Student Registration Form** is a web application built using **HTML**, **CSS**, and **JavaScript**. It allows users to input student details such as **name**, **gender**, **course**, **email**, **skills**, and an optional **image**. Upon submission, the entered data is dynamically displayed in a neatly formatted section on the same page. The form is fully responsive, ensuring a seamless experience across all devices.

---

## ✨ **Features**

- **User-Friendly Form**: A clean and intuitive interface for collecting student details.
- **Dynamic Data Display**: Submitted data is displayed instantly in a structured format.
- **Image Upload**: Option to upload a student's image for a personalized touch.
- **Responsive Design**: Works flawlessly on desktops, tablets, and mobile devices.
- **Form Validation**: Ensures required fields are filled out before submission.
- **Skills Selection**: Allows students to select their skills using checkboxes.

---

## 🛠 **How It Works**

### **HTML Structure**
The `index.html` file defines the structure of the form and the display section. Key components include:
- Input fields for **name**, **course**, **email**, and **image upload**.
- Checkboxes for **gender** and **skills** selection.
- A **submit button** to process the form data.

```html
<form action="" id="form">
    <div class="f1">
        <label for="name">Name*:</label>
        <input type="text" name="name" class="in" placeholder="Enter name" required>
    </div>
    <div class="f2">
        <label for="gender">Gender:</label>
        <div class="c">
            <div class="c1"><input type="checkbox" name="gender">
                <label for="">Male</label>
            </div>
            <div class="c1"><input type="checkbox" name="gender">
                <label for="">Female</label>
            </div>
        </div>
    </div>
    <!-- Additional fields for course, email, skills, and image upload -->
</form>
```

### **JavaScript Functionality**
The `script.js` file handles form submission and dynamically displays the entered data:
- Prevents the default form submission behavior.
- Captures input values and creates new DOM elements to display the data.
- Handles image uploads and displays the uploaded image.

```javascript
form.addEventListener("submit", (e) => {
    e.preventDefault();
    data();
    form.reset();
});
```

### **CSS Styling**
The `style.css` file provides the visual styling for the form and the displayed data:
- Modern and clean design with a dark theme.
- Responsive layout adjustments for smaller screens.

```css
.container {
    background-color: #1f1f1f;
    border-radius: 5px;
    box-shadow: 0 0 15px black;
    padding: 20px;
}
```

---

## 💻 **Technologies Used**

- **HTML**: For structuring the form and display section.
- **CSS**: For styling the form and ensuring responsiveness.
- **JavaScript**: For handling form submission and dynamic data display.

---

## 📥 **Installation**

To use this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/student-registration-form.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd student-registration-form
   ```

3. **Open the Project**:
   - Open the `index.html` file in your preferred browser.

---

## 🖥 **Usage**

1. **Fill Out the Form**:
   - Enter the student's **name**, select **gender**, **course**, **email**, and upload an **image** (optional).
   - Select the student's **skills** from the provided checkboxes.

2. **Submit the Form**:
   - Click the **Submit** button to process the data.

3. **View the Displayed Data**:
   - The submitted data will be displayed in the **Registered Students** section below the form.

---



# WEB TASK 3


# 🧮 **Calculator Web Application** 🧮

Welcome to the **Calculator Web Application**! This is a sleek, responsive, and user-friendly calculator built using **HTML**, **CSS**, and **JavaScript**. Whether you're performing simple arithmetic or complex calculations, this calculator has got you covered. With a clean design, smooth animations, and support for all basic operations, it’s the perfect tool for quick calculations on the go.

---

## 📌 **Table of Contents**
1. [Introduction](#-introduction)
2. [Features](#-features)
3. [Requirements](#-requirements)
4. [Installation](#-installation)
5. [Usage](#-usage)
6. [Code Walkthrough](#-code-walkthrough)

---

## 🚀 **Introduction**

The **Calculator Web Application** is a lightweight yet powerful tool designed to perform basic arithmetic operations like addition, subtraction, multiplication, and division. It also supports advanced operations like percentage calculations and decimal inputs. The app is built with a responsive design, ensuring it works seamlessly on both desktop and mobile devices.

---

## ✨ **Features**

- **Basic Operations**: Perform addition, subtraction, multiplication, and division.
- **Advanced Operations**: Calculate percentages and use decimal points.
- **Clear Functionality**: Clear the input with a single click.
- **Backspace Functionality**: Remove the last entered digit or operator.
- **Responsive Design**: Works flawlessly on all screen sizes.
- **Smooth Animations**: Built with **Animate.css** for a polished user experience.
- **Modern Design**: Stylish buttons and layout powered by **Bootstrap**.

---

## 📋 **Requirements**

- A modern web browser (Chrome, Firefox, Safari, Edge, etc.).
- No additional installations are required—just open the app and start calculating!

---

## 🛠️ **Installation**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/calculator.git
   cd calculator
   ```

2. **Open the Application**:
   - Open the `index.html` file in your browser:
     ```bash
     open index.html
     ```

---

## 🖥️ **Usage**

1. **Enter Numbers**: Click the number buttons (`0-9`) to input numbers.
2. **Perform Operations**: Use the operator buttons (`+`, `-`, `*`, `/`, `%`) to perform calculations.
3. **Clear Input**: Click the `C` button to clear the input field.
4. **Backspace**: Click the backspace button (`←`) to remove the last entered digit or operator.
5. **Calculate Result**: Click the `=` button to compute and display the result.

---

## 🧑‍💻 **Code Walkthrough**

### **HTML Structure**
The `index.html` file defines the structure of the calculator, including the input field and buttons.

```html
<calculator>
    <textbox>
        <input readonly type="text" class="input" id="number" placeholder="Calculate Here">
    </textbox>
    <buttons>
        <row>
            <button type="button" class="btn btn-dark" onclick="getnumber('7')">7</button>
            <button type="button" class="btn btn-dark" onclick="getnumber('8')">8</button>
            <button type="button" class="btn btn-dark" onclick="getnumber('9')">9</button>
            <button type="button" class="btn btn-success" onclick="Clear()">C</button>
        </row>
        <!-- Additional rows for buttons -->
    </buttons>
</calculator>
```

### **CSS Styling**
The `main.css` file provides the visual styling for the calculator, including layout, colors, and responsiveness.

```css
calculator {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 2em;
    border: 0px;
    padding: 3em 1em;
    border-radius: 25px;
    row-gap: 3em;
    background-color: #dadada;
}
```

### **JavaScript Functionality**
The `main.js` file handles the logic for input, calculations, and display.

```javascript
function getnumber(num) {
    let result = document.getElementById("number");
    result.value += num;
}

function Clear() {
    let result = document.getElementById("number");
    result.value = "";
}

function Result() {
    let result = document.getElementById("number");
    result.value = eval(result.value);
}

function Back() {
    var str = document.getElementById('number').value;
    str = str.substr(0, str.length - 1);
    document.getElementById('number').value = str;
}
```

---
