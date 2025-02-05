# Resume Website Documentation :memo:

This resume website is a well-structured digital profile designed to showcase professional experience, skills, and contact information. Below is a detailed breakdown with code examples to help understand the structure.

## 1️⃣ Page Layout with Flexbox and Grid

The layout is divided into two main sections: an aside for contact and education, and a main area for work experience and profile content. The use of `display: grid` and `display: flex` makes the design responsive.

### 💻 CSS Code for Layout
```css
.resume-container {
  display: grid;
  grid-template-columns: 1fr 2fr; /* Sidebar takes 1/3, main takes 2/3 */
  max-width: 60%;
  background: white;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

body {
  display: flex;
  justify-content: center;
  padding: 40px;
}
```
**Explanation:** The grid divides the container into two parts: sidebar (`1fr`) and main content (`2fr`).

---

## 2️⃣ Profile Picture Styling

A circular profile picture helps personalize the website and enhances visual appeal.

### 🖼️ HTML and CSS for Profile Picture
```html
<div class="profile-picture">
  <img src="https://static.vecteezy.com/system/resources/previews/005/544/718/non_2x/profile-icon-design-free-vector.jpg" alt="Profile Picture">
</div>
```
```css
.profile-picture {
  width: 150px;
  height: 150px;
  border-radius: 50%; /* Makes the image circular */
  background-color: white;
  margin: 0 auto 20px auto;
  overflow: hidden;
}
.profile-picture img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```
**Explanation:** `border-radius: 50%` turns the image container into a circle, and `object-fit: cover` ensures the image fits without distortion.

---

## 3️⃣ Contact and Skills Section with Unordered Lists

The aside section contains lists for contact details and skills.

### 📧 HTML Example
```html
<div class="contact-section">
  <h2 class="section-title">Contact</h2>
  <ul>
    <li>📞 +123-456-7890</li>
    <li>📧 richard.sanchez@email.com</li>
    <li>📍 123 Anywhere St, Anytown</li>
  </ul>
</div>
```
### 🎨 CSS Styling for Lists
```css
ul {
  list-style: none; /* Removes default bullet points */
  margin-top: 10px;
}
```
By removing the default bullet points and adding margins, the list becomes cleaner and visually appealing.
