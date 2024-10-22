# Antlers for Sublime Text

Get your hopes down ;)

Various AI assistants and I tinkered with this for an hour without really understanding how Sublime's code parser works. I offer this because [this 6yo repo](https://github.com/addisonhall/antlers-statamic-sublime-syntax) no longer works. I don't want to use VS Code, so I am mildly committed to experiment further, but I hate troubleshooting meta-problems.

## Installation
I manually added these 2 files on my Mac in `~/Library/Application Support/Sublime Text/Packages/User`

## Status:
- The Current two files "work" in that I can comment-out a `{{ tag }}` like `{{# {{ tag }} #}}` (so, double-pairs like VS, not the typical `{{# tag #}}` pair, but whatever) - AND it will uncomment when `cmd+/` is hit again
- Usually I can't uncomment `{{ if show_title }}` (but... I am certain it worked for a bit!? Sometimes restarting Sublime changes stuff, sometimes it doesn't - the inconsistency with some of my troubleshooting is the main reason I have to stop working on this) - what happens is that it stacks the commenting `{{# {{# {{ if show_title }} #}} #}}`
- The Antlers files have no code coloring, the HTML and Antlers tags are all white.

**Funny story:** When I asked ChatGPT 4o for help with commenting / uncommenting I was back and forth making very little progress. Basically, trying to solve this problems was a waste of time. However, when I took ChatGPT up on this offer it fixed my first comments issue 🙄 _"Do you want assistance with additional Antlers-specific syntax highlighting (like loops, conditionals, or custom Statamic tags)?"_
