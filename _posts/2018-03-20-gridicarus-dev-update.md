---
layout: post
title: "Gridicarus: Development Update #1"
category: project
published: true
---

Gridicarus is now stable at ```0.1.5```! This is the *final* "initial commit" for Gridicarus. I've gotten the documentation to a point where I'm happy with the framework, the ```package.json``` file is squared away, and I think it's generally smooth sailing from here. Well, I use smooth sailing loosely... The stuff I wanna implement is not going to be fun.

Anyways, I should probably introduce the framework a little bit since this is the first Development Log.

### What's Gridicarus?

Gridicarus is a CSS framework based around CSS Grids. I designed it to make the already easy CSS Grids even easier. And I think I've done a decent job so far. It does sacrifice *(for now)* some of the functionality of the CSS Grid spec. However, you can quickly develop nice, grid-based websites without even touching CSS! Pretty cool, eh?

However, like any early project, it doesn't come without its pitfalls. For example, it's difficult to create vertical-grid-centric sites since the markup is so focused around horizontal-grid-centricity(?). This is because I only thought of horizontal grid designs while writing the prototype. Not vertical. I found out why this wasn't a good design choice once I started writing the documentation. Needless to say I rewrote a small amount of SCSS...

### Current Plans + The Future

The current plans for Gridicarus are to get the framework to a point where you can mix and match grid layouts using predefined templates.

For example, ```.template1``` could be something like this:  

```css
"header   header   header"   
"sidebar  content  content"  
"footer   footer   footer"
```


Then ```.template-2``` could replace one of the content areas for a second sidebar or remove the sidebar completely. My goal is to make Gridicarus a really quick grid templating framework. One where you can quickly swap out layouts to test new site designs, or even prototype new designs using the premade classes. I want to do this using only CSS, and only CSS Grids.

### What's happening now

As of now, I'm currently adding QOL features. More columns and rows, higher children count, better class naming, etc. Some of which I've already done in ```0.2.0```. You can download it using the CDN link:

    <link rel="stylesheet" href="https://unpkg.com/gridicarus@0.2.0/dist/gridicarus.min.css">

or NPM:

    npm install gridicarus

Note that there is no documentation for ```0.2.0``` yet, so you'll have to make do reading the actual Gridicarus file. There's also legacy support, so if you *(surprisingly)* have a Gridicarus project using ```0.1.5```, you can still use those features and naming conventions, while also using the new and improved ones.

### Closing

Hopefully this was a decent enough DevLog. I don't really ever write these, so if I'm lacking information or something doesn't seem clear, let me know!

Anyways, thanks for reading and I'll talk to you all sometime soon!
