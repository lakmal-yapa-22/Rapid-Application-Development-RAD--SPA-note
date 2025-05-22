# 🧠 Single Page Applications vs Multi Page Applications

## 🏃‍♂️ Rapid Application Development (RAD)
**RAD** කියන්නේ *fast and flexible software development model* එකක්.  
📌 Requirements frequently change වෙන **small/medium projects** සඳහා සුදුසුයි.  
📌 Rapid prototyping + user feedback + iterative refinement = RAD.

---

## 🌐 Web Application Architecture

Web applications develop කරන විදිහට ප්‍රධාන වශයෙන් ආකාර 2ක් තියෙනවා:

- **SPA - Single Page Applications**
- **MPA - Multi Page Applications**

---

## 📄 MPA (Multi Page Application)

> **Definition:**  
An MPA loads a **new HTML page from the server** for each user interaction that requires updated content. This results in a full-page reload every time.

### ❓How MPAs Work
1. User clicks a link ➡️ sends a new request to the server  
2. Server responds with a **complete HTML page**  
3. Browser discards the old page and renders the new one  

### ✅ Advantages
- 🟢 **SEO friendly** – Ideal for search engine indexing  
- 🟢 **Simple architecture** – Especially with server-side rendering  
- 🟢 Best for traditional forms and full-page navigation

### ❌ Disadvantages
- 🔴 **Slow user experience** – Full-page reload on every interaction  
- 🔴 Static files reload each time  
- 🔴 Not suitable for real-time apps

### 🛠️ Typical Tech Stack
- Server-side frameworks: **Django**, **Laravel**, **Spring MVC**, **Ruby on Rails**  
- Templating Engines: **Jinja2**, **Blade**, **Thymeleaf**

---

## 🔄 SPA (Single Page Application)

> **Definition:**  
An SPA loads once with a shell (HTML + JS). After that, it dynamically updates the page content **without reloading**.

### ❓How SPAs Work
1. First load → loads HTML shell + JavaScript bundles  
2. Browser renders the app  
3. User interacts → no page reload  
4. Server calls only for **data (via APIs)**  
5. DOM updates dynamically

### ✅ Advantages
- 🟢 Smooth UX (no reloads)  
- 🟢 Dynamic and rich UI (like mobile apps)  
- 🟢 Efficient — fetches only data, not the whole page

### ❌ Disadvantages
- 🔴 Heavy **initial load**  
- 🔴 **SEO** is tricky – SSR or pre-rendering needed

### 🛠️ Typical Tech Stack
- JS Frameworks: **React**, **Angular**, **Vue.js**  
- Routing: **React Router**, **Vue Router**  
- API: **REST**, **GraphQL**  
- State Management: **Redux**, **Vuex**, **Pinia**  
- Data Format: **JSON**

---

## ⚖️ MPA vs SPA - Summary

| Feature      | MPA                         | SPA                             |
|--------------|-----------------------------|----------------------------------|
| Reload       | Full-page reload            | No reload – dynamic updates     |
| Performance  | Slower (server heavy)       | Faster (client-side rendering)  |
| SEO          | Better                      | Needs SSR / Pre-rendering       |
| Architecture | Server-rendered             | Client-rendered (JS-heavy)      |
| Use Case     | Blogs, E-commerce, Static Sites | Dashboards, Social Media, Admin Apps |

---

