---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.unsplash.com/photo-1619441207978-3d326c46e2c9?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D 
# some information about your slides, markdown enabled
title: Wed Accessibility 
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Introduction about Web Accessibility 
# apply any unocss classes to the current slide
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
---

# Web Accessibility 


Introduction to Web Accessibility 

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# Introduction to Web Accessibility  



---
transition: slide-up
level: 2
---

# Navigation

<Toc v-click minDepth="1" maxDepth="2"></Toc>

---
layout: two-cols
layoutClass: gap-16
---

# Table of contents

You can use the `Toc` component to generate a table of contents for your slides:

```html
<Toc minDepth="1" maxDepth="1"></Toc>
```

The title will be inferred from your slide content, or you can override it with `title` and `level` in your frontmatter.

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
