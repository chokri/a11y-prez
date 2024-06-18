---
theme: apple-basic
title: Web Accessibility
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
---

<Toc minDepth="1" maxDepth="2" />

---
transition: fade-out
layout: image-right
image: assets/handicap_parking_marker.jpg
---

## 1 - What is A11y?

- **A11y** stands for __accessibility__.
- With A11y, people with disabilities can:
  - perceive, understand, navigate, and interact with the Web
  - contribute to the Web

<!--
 It means making sure that everything, from websites to buildings, can be used by as many people as possible. This includes people with disabilities.

- There are rules to help people with disabilities, but it’s important for creators to think about all kinds of users in different situations.

When websites and web tools are properly designed and coded, people with disabilities can:

- perceive, understand, navigate, and interact with the Web
- contribute to the Web
-->

---
transition: fade-out
layout: two-cols
---

## 2 - What kind of disability ?

Web accessibility means making the internet work for everyone, no matter what kind of disability they might have. This includes:

- Visual
- Auditory
- Cognitive
- Neurological
- Physical
- Speech

::right::
<img style="margin-top:30%" src="/assets/building-web-accessibility.jpg" />


<!--
- Visual: Helping people who have trouble seeing.
- Auditory: Making sure people who have difficulty hearing can get information.
- Cognitive: Assisting those with challenges in understanding or processing information.
- Neurological: Supporting users with brain-related conditions.
- Physical: Ensuring those with limited movement can navigate and interact.
- Speech: Helping people with speech disabilities communicate and access content.
-->

---
transition: fade-out
layout: image-right
image: assets/old-lady-crazy.gif
---

## 3 - Everyone is concerned

Web accessibility also benefits people without disabilities, for example:

- people using mobile phones, smart watches, smart TVs, and other devices with small screens, different input modes, etc.
- people with changing abilities due to ageing
- people with “temporary disabilities” such as a broken arm or lost glasses


---
transition: fade-out
layout: image-right
image: assets/Disabled-Student-Working.jpg
---

## 4 - Web Accessibility Tools

- **Screen Narrators**
- **Braille Readers**
- **Mouth Sticks**
- **Head Wand**
- **Single-switch access**
- **Sip and puff Sitch**
- **Oversized trackball mouse**
- **Adaptive Keyboard**
- **Eye tracking glasses**
- **Voice recording software**

<!-- These tools play a crucial role in making technology accessible and usable for individuals with various disabilities -->

---
layout: section
---

# Accessibility In Practice

---
transition: fade-out
---

## 1 - Use Skip Menu

**Skip link** to allow users to bypass repeated navigation content

```html {all|5|all} twoslash
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

## 2 - Use Semantic HTML

Semantic HTML elements like `<article>`, `<nav>`, `<section>`, and `<aside>` provide meaningful information about the content of a page, which is especially helpful for screen readers and other assistive technologies. This makes web content more accessible to people with disabilities.

```html {all|1|2|3|all} twoslash
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

## 3 - Use area-label

The `role` and `aria-label` attributes help assistive technologies understand the purpose of the element.

```html {all|2|12|all} twoslash
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

## 4 - Use Keyboard Navigation

With `onkeypress` the link can be activated using the keyboard, not just with a mouse click.

```html
<a href="#" onclick="openMenu()" onkeypress="openMenu()">Open Menu</a>
```

---
layout: section
---

# Accessibility Standards

---
transition: fade-out
---


## Web Content Accessibility Guidelines (WCAG)
<a target="_blank" href="https://www.w3.org/WAI/standards-guidelines/wcag/" alt="WCAG">WCAG</a> specifies three different conformance levels they are:

- A (lowest)
- AA (mid range)
- and AAA (highest)

>  Level A sets a minimum level of accessibility and does not achieve broad accessibility for many situations. For this reason, UC recommends AA conformance for all Web-based information.

---
transition: fade-out
---

## WebAIM

<a target="_blank" href="https://webaim.org/">WebAIM</a> provides a handy checklist with their recommendations.

WebAIM specifies that accessible websites should be:

- Perceivable
- Operable
- Understandable
- Robust

---
transition: fade-out
---

## Links

- <a href="https://accessibility.day/" target="_blank"> The GAAD Foundation</a>
- <a href="https://www.w3.org/WAI/design-develop/" target="_blank">w3.org</a>
- <a href="https://react-spectrum.adobe.com/react-spectrum/" target="_blank">React Spectrum</a>
- <a href="https://inclusive.microsoft.design/" target="_blank">Microsoft</a>
- <a href="https://pagespeed.web.dev/" target="_blank">Web.dev</a>

- <a href="https://www.npmjs.com/package/eslint-plugin-jsx-a11y" target="_blank">eslint-plugin-jsx-a11y</a>

---
transition: fade-out
layout: center
---

# Thank you

<a href="https://github.com/chokri" target="_blank" alt="GitHub" title="Open GitHub"
    class="text-xl opacity-50 !border-none">
    <carbon-logo-github /> chokri
</a>

<a href="https://twitter.com/shuck_" target="_blank" alt="Twitter" title="Open Twitter"
    class="text-xl opacity-50 !border-none">
    <carbon-logo-twitter /> @shuck_
</a>
