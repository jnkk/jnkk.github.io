---
title: Index for learning in my Personal Notes on Github pages
tags: index, 
---

# Learning

> [!NOTE] NOTE TO SELF
> Cleaning files and folders of this might be an order. For better site mapping.  
> BUT before that, github actions failed to "execute" because IDK how to use and messed up the `MERGE` thingy in the `Pull Request` thingy. Can't fixed it. Maybe just moving `content` folder and restart it again.  
> So, right now it is just a note taking provider inside Github. Also in Google Drive. But not as up to date as in Github.

Go to the directory note-pages/content
This is the `index.md` file. In the root directory.

## [[Latest]](Notes/notesgithubpages.md)  

## [[After install]](./Notes/afterinstallDEBIAN.md)

## [Selfhost](Selfhost/Selfhost.md) [Link](https://selfh.st/)

### TODOs  

In dire need of a new pc. 8 core, 16 threads with a minimum of 32 GBs of RAM and 16 GBs of VRAM like the Radeon 7600 XT. So I can run [ollama](https://ollama.com/)/LLMs locally using [continuedev](https://github.com/continuedev/continue) inside VSCode. Playing around with local LLMs right now can be an advatage in the future where it is everywhere.
Local agentic LLMs using programs like [Autogen](https://github.com/microsoft/autogen) might be helpful for local "AI helpers".

The component list inside
[Proxmox Server](https://pcpartpicker.com/list/qqnKPF)
is "ideal" for starters, maybe overkill for beginners LMAO.

Customizing the "front page" to display folder files

#### This is a blank Quartz installation.

See the [documentation](https://quartz.jzhao.xyz) for how to get started

Or see the note-pages directory

### [Cloning notes-personal or "My Digital Garden" with steps:](Notes/notesgithubpages.md)

### Start the server

```bash
npx quartz build --serve
```

### Resync with github pages

```bash
npx quartz sync --no-pull
```
