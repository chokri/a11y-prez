---
theme: apple-basic
background: https://images.unsplash.com/photo-1619441207978-3d326c46e2c9?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
title: Wed Accessibility
info: |
  Presentation slides for developers.

  Introduction about Web Accessibility
class: text-center
highlighter: shiki
drawings:
  persist: false
transition: slide-left
mdc: true
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
layoutClass: gap-16
---

Web accessibility relies on several components that work together. Some of these include:

- Web content - refers to any part of a website, including text, images, forms, and multimedia, as well as any markup code, scripts, applications, and such.
- User agents - software that people use to access web content, including desktop graphical browsers, voice browsers, mobile phone browsers, multimedia players, plug-ins, and some assistive technologies.
- Authoring tools - software or services that people use to produce web content, including code editors, document conversion tools, content management systems, blogs, database scripts, and other tools.

--
layout: two-cols
layoutClass: gap-16
---


Web accessibility relies on several components that work together. Some of these include:

- Web content - refers to any part of a website, including text, images, forms, and multimedia, as well as any markup code, scripts, applications, and such.
- User agents - software that people use to access web content, including desktop graphical browsers, voice browsers, mobile phone browsers, multimedia players, plug-ins, and some assistive technologies.
- Authoring tools - software or services that people use to produce web content, including code editors, document conversion tools, content management systems, blogs, database scripts, and other tools.


::right::

Okey, this text is on the right, righ?

---
layout: image-right
image: https://cover.sli.dev
---

# Code

Use code snippets and get the highlighting directly, and even types hover![^1]

```ts {all|5|7|7-8|10|all} twoslash
// TwoSlash enables TypeScript hover information
// and errors in markdown code blocks
// More at https://shiki.style/packages/twoslash

import { computed, ref } from 'vue'

const count = ref(0)
const doubled = computed(() => count.value * 2)

doubled.value = 2
```

---
layout: image-right
image: https://cover.sli.dev
---

# Example of HTML

Use code snippets and get the highlighting directly, and even types hover![^1]

```html {all|1|3|6|all} twoslash
<div role="navigation" aria-label="Primary">
  <ul>
    <li>...a list of links here ...</li>
  </ul>
</div>
<div role="navigation" aria-label="Secondary">
  <ul>
    <li>...a list of links here ...</li>
  </ul>
</div>
```


---
transition: fade-out
---

# Thank you
