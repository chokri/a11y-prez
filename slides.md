---
theme: apple-basic
title: Wed Accessibility
info: |
  Introduction about Web Accessibility
class: text-center
highlighter: shiki
drawings:
  persist: false
transition: fade-out
mdc: true
layout: center
---

# Introduction to Web Accessibility


---
transition: fade-out
layout: image-right
image: assets/handicap_parking_marker.jpg
---

## What is A11y ?

- Accessibility is the concept of whether a product or service can be used by everyone, regardless of how they encounter it.

- While accessibility laws exist to aid people with disabilities, designers should strive to accommodate all potential users in various contexts of use.


---
transition: fade-out
---


 When websites and web tools are properly designed and coded, people with disabilities can:

- perceive, understand, navigate, and interact with the Web
- contribute to the Web


---
transition: fade-out
---

Web accessibility encompasses all disabilities that affect access to the Web, including:

  - visual
  - auditory
  - cognitive
  - neurological
  - physical
  - speech

<img width="500" src="assets/building-web-accessibility-barriers-guidelines-standards_01.jpg">

---
transition: fade-out
---

Web accessibility also benefits people without disabilities, for example:

- people using mobile phones, smart watches, smart TVs, and other devices with small screens, different input modes, etc.
- older people with changing abilities due to ageing
- people with “temporary disabilities” such as a broken arm or lost glasses


---
transition: fade-out
---

Web accessibility relies on several components that work together. Some of these include:

- **Web content** - refers to any part of a website, including text, images, forms, and multimedia, as well as any markup code, scripts, applications, and such.

- **User agents** - software that people use to access web content, including desktop graphical browsers, voice browsers, mobile phone browsers, multimedia players, plug-ins, and some assistive technologies.

- **Authoring tools** - software or services that people use to produce web content, including code editors, document conversion tools, content management systems, blogs, database scripts, and other tools.

---
transition: fade-out
layout: image-right
image: assets/Disabled-Student-Working.jpg
---

# Assitive Technologies

These tools play a crucial role in making technology accessible and usable for individuals with various disabilities

- **Screen Narrators**
- **Braille Readers**
- **Mouth Sticks**
- **Head Wand**
- **Signle-switch access**
- **Sip and puff Sitch**
- **Oversized trackball mouse**
- **Adaptive Keyboard**
- **Eye tracking glasses**
- **Voice recording software**

---
layoutClass: gap-16
---

Web accessibility relies on several components that work together. Some of these include:

- Web content - refers to any part of a website, including text, images, forms, and multimedia, as well as any markup code, scripts, applications, and such.
- User agents - software that people use to access web content, including desktop graphical browsers, voice browsers, mobile phone browsers, multimedia players, plug-ins, and some assistive technologies.
- Authoring tools - software or services that people use to produce web content, including code editors, document conversion tools, content management systems, blogs, database scripts, and other tools.


---
transition: fade-out
layout: image-right
image: assets/handicap_parking_marker.jpg
---

## How?

---
layout: image-right
image: https://cover.sli.dev
---

# Skip Menu

**Skip link** to allow users to bypass repeated navigation content

```html {all|1|3|6|all} twoslash
<header role="banner">
    <h1>Accessible Blog</h1>
    <nav role="navigation">
        <ul>
            <li><a href="#maincontent">Skip to main content</a></li>
            <!-- Other navigation items -->
        </ul>
    </nav>
</header>
```

---
transition: fade-out
---

# Use Semantic HTML

Semantic HTML elements like `<article>`, `<nav>`, `<section>`, and `<aside>` provide meaningful information about the content of a page, which is especially helpful for screen readers and other assistive technologies. This makes web content more accessible to people with disabilities.

```html {all|1|3|6|all} twoslash
<main id="maincontent" role="main">
    <article aria-labelledby="posttitle">
        <header>
            <h2 id="posttitle">Making Accessibility a Priority</h2>
            <p><time datetime="2024-05-20">May 20, 2024</time></p>
        </header>
        <section>
            <h3>Introduction</h3>
            <p>Accessible web design is essential for all users...</p>
        </section>
        <footer>
            <p>Posted by <a href="#authorbio" aria-describedby="authorname">Alex Doe</a></p>
        </footer>
    </article>
    ...
```

---
transition: fade-out
---

# Use area-label

The `role` and `aria-label` attributes help assistive technologies understand the purpose of the element.

```html {all|1|3|6|all} twoslash
<main id="maincontent" role="main">
    <article aria-labelledby="posttitle">
        <header>
            <h2 id="posttitle">Making Accessibility a Priority</h2>
            <p><time datetime="2024-05-20">May 20, 2024</time></p>
        </header>
        <section>
            <h3>Introduction</h3>
            <p>Accessible web design is essential for all users...</p>
        </section>
        <footer>
            <p>Posted by <a href="#authorbio" aria-describedby="authorname">Alex Doe</a></p>
        </footer>
    </article>
    ...
```


---
transition: fade-out
---

# Use Keyboard Navigation

With `onkeypress` the link can be activated using the keyboard, not just with a mouse click.

```html
<a href="#" onclick="openMenu()" onkeypress="openMenu()">Open Menu</a>
```

---
transition: fade-out
layout: center
---

# Thank you
