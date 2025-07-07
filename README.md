# Web

---

## ✅ 1 – Is this a website or a web app?

### 🌐 *World of web development:* 
From networking fundamentals to modern full-stack technologies.

- A *static website* presents unchanging content that doesn't change unless modified by the developer.
- While an *interactive web* application allows for user interaction, modifying the content and offering dynamic functionality.

### 🌟 *Informative websites:*
An informational website is one whose primary objective is to provide the user with information on a specific topic, whether through text, images, videos, or other formats.

Examples of *informative websites:*

1. Digital magazines like the BBC
2. News portals such as Google News
3. Tutorial and course websites like Coursera

### ✨ *Web applications:*
An app website is a program that runs in a web browser and does not require installation on the user's device.

Examples of *web applications:*

1. Email services like Gmail
2. Social media like Instagram
3. E-commerce platforms like Amazon

#### Summary:
- *Informational websites:* Their primary function is to display information. Interaction is basic (browsing, reading, searching). The content is primarily static.
- *Web applications:* They allow complex tasks, creating and modifying content, managing personal data, and maintaining user states.

#### What makes a web application interactive?
An interactive web application allows users not only to view content but also to interact with it, modifying it and receiving responses in real time.

#### What technologies might be behind it?
This is achieved through the combination of front-end and back-end technologies that work together to create a dynamic experience. Key technologies include HTML, CSS, JavaScript, front-end frameworks like React or Angular, and back-end languages ​​like Python, Ruby, Java, or Node.js, along with databases and APIs.

---

## ✅ 2 – Anatomy of a modern web application

A web application is primarily composed of three parts: 

- ◀️ Frontend: is the part the user sees and interacts with.
- ▶️ Backend: is the server logic and data management.
- 💾 Database: stores the information used by the application.

The communication scheme between the frontend, backend, and database can be described as a conversation where the frontend, the visible part of an application, requests information from the backend, which processes the request and accesses the database to obtain the necessary data, and finally, the backend returns the information to the frontend to be presented to the user.

#### *Web Application Communication Diagrama:* 

![alt text](../../../../Downloads/WebCommunicationDiagram.png)

---

## ✅ 3 – Exploring development tools

### *Browser Devtools:*

Browser development tools, also known as DevTools, are a set of tools built into modern web browsers that allow developers to inspect, debug, and modify the content of a web page in real time. 

They are essential for web development, as they allow for analyzing and troubleshooting HTML, CSS, and JavaScript code, as well as the page's network activity.

### ❓ How to open DevTools:
   - **Windows:** `F12` o `Ctrl + Shift + I`
   - **Linux:** `Ctrl + Shift + I`
   - **Mac:** `Cmd + Option + I`

### 🔎 DevTools Inspection - Google.com:

#### 📑 Elements Tab:

![alt text](../../../../Downloads/Inspecting_an_image.png)

During the inspection in the Elements tab, I identified the button corresponding to the user's login or profile. This is an <a> element (hyperlink) with several characteristics:

🔹 Relevant information:

- Element type: <a> (link that acts as a button)
- CSS class: gb_B gb_Za
- aria-label attribute: Describes the accessible content of the button. In this case, it displays the account name and associated email address.
- Function: When clicked, it displays account options or allows you to log out of Google.

#### 🕹️ Console Tab:

![alt text](../../../../Downloads/warning.png)

- I saw an informational message appearing in the DevTools Console tab referring to a change in Chrome's privacy policies
- I was able to execute JavaScript commands like console.log("Hello world")

#### 🌐 Network Tab: 

Captured HTTP Request!

![alt text](../../../../Downloads/Inspecting_an_HTTP_request.png)

- Name: account?eom=...
- Status: 200 OK
- Type: document
- Size: 27.6 kB
- Time: 132 ms

📍 This is a document request, indicating that it is the main HTML file loaded from the server.

#### 🗃️ Storage Tab:

![alt text](../../../../storageTab.png)

I saw Google cookies with session information
I identified localStorage with user preferences
I observed browser cache data

---

## ✅ 4 – HTML, CSS y JS

### 🔗 **HTML**

HTML or HyperText Markup Language is the fundamental language for creating web pages. It defines the structure and content of a page, including text, images, links, videos, and other multimedia elements, allowing browsers to interpret and display them correctly.

```html
<html>
  <head>
    <title>My first page</title>
  </head>
  <body>
    <h1>Hello world!</h1>
    <p>This is my first paragraph.</p>
    <button>Click me</button>
  </body>
</html>
```

### 🎨 **CSS**

Cascading Style Sheets, is used to define the visual appearance of HTML documents, separating content from presentation. In other words, CSS controls how a web page looks: colors, fonts, margins, layout, etc., while HTML defines the structure of the content.

```css
h1 {
    color: blue;
    font-size: 28px;
    text-align: center;
}

button {
    background-color: green;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
}
```

### 🚀‌ **JavaScript**

JavaScript is a scripting language primarily used to add interactivity and dynamic content to web pages, allowing you to create visual effects, animations, and manipulate page content without reloading the page. It is essential for modern web development, enabling the creation of interactive web applications and client-side data validation.

```javascript
function greet() {
    alert("Hello from JavaScript!");
}

document.getElementById("myButton").onclick = function() {
    console.log("Button clicked!");
};
```

#### Summary:

HTML is the skeleton of a web page, providing the basic structure and content, while CSS and JavaScript handle the appearance and behavior. 

### ⚔️ Java vs JavaScript

![alt text](../../../../JAVA-JS.png)

### ✨ ~ How they are similar:

- **Similar syntax:** Loops, conditionals, and functions are written similarly
- **Object-oriented:** Both handle objects (although JavaScript is more flexible)
- **Variables and functions:** Familiar concepts I already know
- **Programming logic:** Algorithms and control structures are similar

### ✨ ≠ How they differ:

| Java | JavaScript |
|------|------------|
| Needs compilation | Runs directly |
| Static typing (`int x = 5;`) | Dynamic typing (`let x = 5;`) |
| Stricter with errors | More permissive |
| Mainly backend | Mainly frontend |
| Runs on JVM | Runs in browser |

### Example that helped me understand:

♨️ **In Java:**
```java
public class Calculator {
    public static int add(int a, int b) {
        return a + b;
    }
    
    public static void main(String[] args) {
        System.out.println(add(5, 3));
    }
}
```

🟨 **In JavaScript:**
```javascript
function add(a, b) {
    return a + b;
}

console.log(add(5, 3));
```

#### 🤔 Reflection

As someone coming from Java, I'm surprised by how **flexible** JavaScript is. I don't need to declare variable types or compile code. This can be liberating but also requires more discipline.

The concept that caught my attention most is how **HTML, CSS, and JavaScript work together**:
- HTML provides the content
- CSS makes it look good
- JavaScript makes it interactive

It's like Java being the car's engine (backend) and these three technologies being the dashboard, body, and controls (frontend) that the user sees and uses.

---