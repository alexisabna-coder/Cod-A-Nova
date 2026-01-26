# Developer Manual – CodA-Nova Navbar Menu-2

## 1. Project Overview
CodA-Nova is a clean and responsive navigation bar built using **HTML5** and **CSS3**.  
This template is part of the **CodA-Nova UI Series** and is designed to be lightweight, responsive, and easy to customize.

**Technologies used:** HTML5, CSS3 (Flexbox, Media Queries)  
**Planned features:** JavaScript interactivity, Bootstrap integration, PHP backend support

---

## 2. File Structure

CodA-Nova/
│
├── index.html # Main HTML file with navbar
├── README.md
├── assets/
│   ├── css/
│   │   └── style.css # CSS file for design and layout
│   └── prototypes/ screenshots of mobile and desktop layouts for reference
│       ├── Mobile.png
│       └── Navbar_Desktop.png
└── documentation/
    ├── Project_Specifications.md
    ├── User_Manual.md
    ├── Developer_Manual.md



---

## 3. HTML Structure

```html
<header>
  <nav>
    <a href="index.html" class="logo">Cod'A-Nova</a>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="About.html">About</a></li>
      <li><a href="Portfolio.html">Portfolio</a></li>
      <li><a href="Contact.html">Contact</a></li>
      <li><a href="Blog.html">Blog</a></li>
    </ul>
  </nav>
</header>
```


Structure Diagram

```
<nav>
├── <a class="logo">Logo</a>
└── <ul>
    ├── <li><a>Home</a></li>
    ├── <li><a>About</a></li>
    ├── <li><a>Portfolio</a></li>
    ├── <li><a>Contact</a></li>
    └── <li><a>Blog</a></li>
    </ul>
</nav>  ```

4. CSS Overview
```/* Navbar */
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  padding: 20px 40px;
}

nav .logo,
nav ul li a {
  color: #fff;
  text-decoration: none;
  padding: 8px 12px;
  border-radius: 4px;
  transition: all 0.3s ease;
}

/* Hover */
nav .logo:hover,
nav ul li a:hover {
  color: #00bfff;
  background-color: #555;
}
```

5. Adding a New Menu Item
Open index.html.

Add a new <li><a href="...">New Link</a></li> inside <ul>.

Save the file.

Update style.css if needed (colors, spacing, hover).

6. Customization
Change logo text or image in <a class="logo">.

Update menu links in <ul>.

Modify colors, fonts, and spacing in style.css.

7. Notes for Developers
Mobile-first responsive design.

Hover effects only work on desktop.

No JavaScript is needed for basic functionality.

Code is commented line by line

Can evolve with JS, Bootstrap, or PHP backend later