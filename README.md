<br>
<p align="center">
<a href="https://sli.dev" target="_blank">
<img src="https://sli.dev/logo-title.png" alt="Slidev" height="250" width="250"/>
</a>
</p>

<p align="center">
Presentation <b>slide</b>s for <b>dev</b>elopers 🧑‍💻👩‍💻👨‍💻
</p>

<p align="center">
<a href="https://www.npmjs.com/package/@slidev/cli" target="__blank"><img src="https://img.shields.io/npm/v/@slidev/cli?color=2B90B6&label=" alt="NPM version"></a>
<a href="https://www.npmjs.com/package/@slidev/cli" target="__blank"><img alt="NPM Downloads" src="https://img.shields.io/npm/dm/@slidev/cli?color=349dbe&label="></a>
<a href="https://sli.dev/" target="__blank"><img src="https://img.shields.io/static/v1?label=&message=docs%20%26%20demos&color=45b8cd" alt="Docs & Demos"></a>
<a href="https://sli.dev/resources/theme-gallery" target="__blank"><img src="https://img.shields.io/static/v1?label=&message=themes&color=4ec5d4" alt="Themes"></a>
<br>
<a href="https://github.com/slidevjs/slidev/stargazers" target="__blank"><img alt="GitHub stars" src="https://img.shields.io/github/stars/slidevjs/slidev?style=social"></a>
</p>

<p align="center">
  <a href="https://twitter.com/antfu7/status/1389604687502995457">Video Preview</a> | <a href="https://sli.dev">Documentation</a>
</p>

<div align="center">
<table>
<tbody>
<td align="center">
<img width="2000" height="0" alt="" aria-hidden><br>
<sub>Made possible by my <a href="https://github.com/sponsors/antfu">Sponsor Program 💖</a></sub><br>
<img width="2000" height="0" alt="" aria-hidden>
</td>
</tbody>
</table>
</div>

## Features

- 📝 [**Markdown-based**](https://sli.dev/guide/syntax) - focus on content and use your favorite editor
- 🧑‍💻 [**Developer Friendly**](https://sli.dev/guide/syntax#code-blocks) - built-in code highlighting, live coding, etc.
- 🎨 [**Themable**](https://sli.dev/resources/theme-gallery) - theme can be shared and used with npm packages
- 🌈 [**Stylish**](https://sli.dev/guide/syntax#embedded-styles) - on-demand utilities via [UnoCSS](https://github.com/unocss/unocss).
- 🤹 [**Interactive**](https://sli.dev/custom/directory-structure#components) - embedding Vue components seamlessly
- 🎙 [**Presenter Mode**](https://sli.dev/guide/ui#presenter-mode) - use another window, or even your phone to control your slides
- 🎨 [**Drawing**](https://sli.dev/features/drawing) - draw and annotate on your slides
- 🧮 [**LaTeX**](https://sli.dev/features/latex) - built-in LaTeX math equations support
- 📰 [**Diagrams**](https://sli.dev/guide/syntax#diagrams) - creates diagrams using textual descriptions with [Mermaid](https://mermaid.js.org/)
- 🌟 [**Icons**](https://sli.dev/features/icons) - access to icons from any icon set directly
- 💻 [**Editor**](https://sli.dev/guide/index#editor) - integrated editor, or the [VSCode extension](https://sli.dev/features/vscode-extension)
- 🎥 [**Recording**](https://sli.dev/features/recording) - built-in recording and camera view
- 📤 [**Portable**](https://sli.dev/guide/exporting) - export into PDF, PNGs, or PPTX
- ⚡️ [**Fast**](https://vitejs.dev) - instant reloading powered by [Vite](https://vitejs.dev)
- 🛠 [**Hackable**](https://sli.dev/custom/) - using Vite plugins, Vue components, or any npm packages

## 🤖 LLM-Powered Enhancements

### 1. Auto-Generate Slides from Content
Transform articles, documentation, or any text content into presentation slides automatically.

```javascript
// CLI tool: paste article/docs → get slides
// "Summarize this into 10 slides with key points"
npx slidev-ai generate --input article.md --slides 10
```

### 2. Voice-to-Slides
Record your talk idea and let AI generate draft slides from your speech.

```javascript
// Whisper API → transcript → LLM → slides.md
// "Record your talk idea, get draft slides"
npx slidev-ai voice --output my-talk.md
```

### 3. Smart Speaker Notes
LLM generates comprehensive presenter notes including talking points, timing estimates, and predicted Q&A.

```javascript
// Analyze slides and generate rich speaker notes
npx slidev-ai notes --input slides.md --timing --qa-prep
```

### 4. Real-time Q&A Component
Embed an AI-powered Q&A system directly into your presentation for live audience interaction.

```vue
<template>
  <!-- Audience asks questions → AI answers based on slide context -->
  <SlidevAIChat :context="slideContent" />
</template>
```

### 5. Auto-Styling & Theme Suggestions
Let AI analyze your content and recommend the perfect theme, colors, and layouts.

```javascript
// Analyze content → suggest appropriate theme, colors, layouts
// "Technical content detected → use 'seriph' theme with code focus"
npx slidev-ai theme --input slides.md --suggest
```

### 6. Content Enhancement
AI-powered suggestions to improve your slides with diagrams, code examples, and better titles.

```javascript
// "Add relevant Mermaid diagram for this concept"
// "Generate code example for this explanation"
// "Suggest better title for this slide"
npx slidev-ai enhance --input slides.md --diagrams --examples
```

## Getting Started

### Try it Online ⚡️

[sli.dev/new](https://sli.dev/new)

[![](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://sli.dev/new)

### Init Project Locally

Install [Node.js >=18](https://nodejs.org/) and run the following command:

```bash
npm init slidev
```

Documentation:
**[English](https://sli.dev)** | [中文文档](https://cn.sli.dev) | [Français](https://fr.sli.dev) | [Español](https://es.sli.dev) | [Русский](https://ru.sli.dev) | [Português-BR](https://br.sli.dev)

Discord: [chat.sli.dev](https://chat.sli.dev)

For a full example, you can check the [demo](https://github.com/slidevjs/slidev/blob/main/demo) folder, which is also the source file for [my previous talk](https://antfu.me/posts/composable-vue-vueday-2021).

## Tech Stack

- [Vite](https://vitejs.dev) - An extremely fast frontend tooling
- [Vue 3](https://v3.vuejs.org/) powered [Markdown](https://daringfireball.net/projects/markdown/syntax) - Focus on the content while having the power of HTML and Vue components whenever needed
- [UnoCSS](https://github.com/unocss/unocss) - On-demand utility-first CSS engine, style your slides at ease
- [Shiki](https://github.com/shikijs/shiki), [Monaco Editor](https://github.com/Microsoft/monaco-editor) - First-class code snippets support with live coding capability
- [RecordRTC](https://recordrtc.org) - Built-in recording and camera view
- [VueUse](https://vueuse.org) family - [`@vueuse/core`](https://github.com/vueuse/vueuse), [`@vueuse/motion`](https://github.com/vueuse/motion), etc.
- [Iconify](https://iconify.design/) - Icon sets collection.
- [Drauu](https://github.com/antfu/drauu) - Drawing and annotations support
- [KaTeX](https://katex.org/) - LaTeX math rendering.
- [Mermaid](https://mermaid-js.github.io/mermaid) - Textual Diagrams.

## Sponsors

This project is made possible by all the sponsors supporting my work:

<p align="center">
  <a href="https://github.com/sponsors/antfu">
    <img src='https://cdn.jsdelivr.net/gh/antfu/static/sponsors.svg' alt="Logos from Sponsors" />
  </a>
</p>

## License

MIT License © 2021 [Anthony Fu](https://github.com/antfu)
