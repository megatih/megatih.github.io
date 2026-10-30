---
layout: post
title: "Cheetah3D Meets AI"
subtitle: "Introducing c3d-mcp: tell an AI what to build, and watch it appear in Cheetah3D"
cover-img: /assets/img/c3d-mcp/cover.jpg
thumbnail-img: /assets/img/c3d-mcp/cyberpunk-cheetah-final.jpg
share-img: /assets/img/c3d-mcp/cover.jpg
tags: [cheetah3d, mcp, ai, 3d, macos, claude, codex, antigravity, projects]
description: "c3d-mcp lets an AI assistant build, light and render scenes inside Cheetah3D on your Mac. A friendly guide with one-command install and two benchmark scenes: a Cornell Box and a Cyberpunk Diorama."
comments: true
---

<style>
  .c3d-lead { font-size: 1.35rem; line-height: 1.5; font-weight: 500; margin: 0.5rem 0 1.5rem; }
  .c3d-card { border: 1px solid rgba(127,127,127,.35); border-radius: 12px; padding: 1rem 1.25rem; margin: 1.25rem 0; background: rgba(127,127,127,.06); }
  .c3d-card p:last-child { margin-bottom: 0; }
  .c3d-table { width: 100%; border-collapse: collapse; margin: 1.25rem 0; font-size: 0.95rem; }
  table.c3d-table, table.c3d-table tr, table.c3d-table th, table.c3d-table td { background: transparent !important; color: inherit !important; }
  table.c3d-table { border: 0; }
  .c3d-table th, .c3d-table td { padding: .6rem .75rem; text-align: left; vertical-align: top; border: 0; border-bottom: 1px solid rgba(127,127,127,.3); }
  .c3d-table th { font-size: .8rem; text-transform: uppercase; letter-spacing: .04em; opacity: .75; }
  .c3d-table td:first-child { font-weight: 600; white-space: nowrap; }
  @media (max-width: 640px) {
    .c3d-table, .c3d-table tbody, .c3d-table tr, .c3d-table td { display: block; width: 100%; }
    .c3d-table thead { display: none; }
    .c3d-table tr { padding: .5rem 0; border-bottom: 1px solid rgba(127,127,127,.3); }
    .c3d-table td { border: 0; padding: .15rem 0; white-space: normal !important; }
  }
  .c3d-steps { counter-reset: step; list-style: none; padding: 0; margin: 1.25rem 0; }
  .c3d-steps li { counter-increment: step; position: relative; padding: .9rem 1rem .9rem 3.6rem; margin-bottom: .75rem; border: 1px solid rgba(127,127,127,.35); border-radius: 12px; background: rgba(127,127,127,.06); }
  .c3d-steps li::before { content: counter(step); position: absolute; left: 1rem; top: .85rem; width: 1.9rem; height: 1.9rem; border-radius: 50%; background: #7c4dff; color: #fff; font-weight: 700; text-align: center; line-height: 1.9rem; }
  figure.c3d-fig { margin: 1.5rem 0; text-align: center; }
  figure.c3d-fig img { max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 18px rgba(0,0,0,.25); }
  figure.c3d-fig figcaption { font-size: .9rem; opacity: .8; margin-top: .6rem; line-height: 1.4; }
  .c3d-pair { display: flex; align-items: flex-start; gap: 1rem; }
  .c3d-pair figure.c3d-fig { margin: 0; min-width: 0; }
  .c3d-pair figure.c3d-fig img { display: block; width: 100%; height: auto; }
  @media (max-width: 640px) { .c3d-pair { flex-direction: column; align-items: stretch; } .c3d-pair figure.c3d-fig { flex: none !important; } }
  .c3d-cmd { font-family: ui-monospace, SFMono-Regular, Menlo, monospace; font-size: .9rem; word-break: break-all; }
  .c3d-btns { text-align: center; margin: 1.5rem 0; }
  .c3d-btns a { margin: .25rem; }
</style>

<p class="c3d-lead"><strong>c3d-mcp</strong> lets an AI assistant build, light and render scenes inside Cheetah3D on your Mac, while you simply describe what you want in plain English.</p>

<div class="c3d-btns">
  <a class="btn btn-primary btn-lg" href="https://github.com/megatih/c3d-mcp">Get c3d-mcp on GitHub</a>
  <a class="btn btn-outline-primary btn-lg" href="#install-in-5-easy-steps">Jump to the install steps</a>
</div>

## How this all started

I have been a Cheetah3D user for many years. It has always been my go-to 3D app on the Mac: it is easy to use, it never gets in my way, and it produces great results.

Recently I kept seeing people get amazing results by connecting AI assistants to Blender through something called *Blender MCP*. I couldn't help wishing that Cheetah3D could do the same.

I knew Cheetah3D can run JavaScript macros, but I had never really explored that feature. Honestly, I found it too difficult to use and understand. That changed with the help of AI. Once an AI could write and explain the scripts for me, a door opened, and **c3d-mcp** is what came through it.

<div class="c3d-card">
<p><strong>What is MCP?</strong> It stands for <em>Model Context Protocol</em>: a standard way for AI apps (like Claude, Codex or Antigravity) to use other apps as tools. With c3d-mcp, Cheetah3D becomes a tool your AI can pick up and use.</p>
</div>

## What you get

<table class="c3d-table">
  <thead><tr><th>What you get</th><th>What it means for you</th><th>Example</th></tr></thead>
  <tbody>
    <tr><td>Talk to Cheetah3D</td><td>Describe the scene in everyday words. The AI does the clicking, scripting and typing for you.</td><td>"Build a small dining table with a wood top and four legs."</td></tr>
    <tr><td>Build scenes fast</td><td>Basic shapes, custom models, pipes, folders, even hundreds of objects at once.</td><td>"Add 140 paving stones, each slightly different."</td></tr>
    <tr><td>Materials and textures</td><td>Wood, marble, glass, metal, glowing neon, and different materials on different parts of one object.</td><td>"Make the sphere polished chrome and the vase gold."</td></tr>
    <tr><td>Lights, cameras and backgrounds</td><td>Studio-style lighting and framing, with automatic checks that the picture is not too dark or empty.</td><td>"Add a warm key light and a soft purple backdrop."</td></tr>
    <tr><td>It looks at its own work</td><td>The AI renders a picture, studies it, and fixes its own mistakes. Optional finishing touches add glow, outlines and colour grading.</td><td>"Render it, tell me what looks wrong, then fix it."</td></tr>
    <tr><td>Animation and export</td><td>Keyframe animation, image sequences, and export to common formats such as FBX, DAE, STL and USDZ. It can also fetch free models from Poly Haven.</td><td>"Spin the model slowly and export it as FBX."</td></tr>
    <tr><td>Safe by design</td><td>Works in a fresh scratch document, never overwrites your files, takes automatic checkpoints you can roll back to, and asks before anything risky.</td><td>"Undo that, go back to the checkpoint before the roof."</td></tr>
    <tr><td>Easy to install</td><td>One command sets everything up, and the same command later updates, repairs or removes it. Works with Claude, Codex and Antigravity (and others), and comes with "skills" that teach your AI how to get the best out of it.</td><td>See the five steps below.</td></tr>
  </tbody>
</table>

## What you need

- A **Mac** with macOS 14 or newer.
- **Cheetah3D 8.1.3** (installed, and opened at least once). Get it from the [official Cheetah3D website](https://www.cheetah3d.com).
- An **AI app that supports MCP**, for example Claude Desktop, Claude Code, Codex or Antigravity.

## Install in 5 easy steps

<ol class="c3d-steps">
  <li><strong>Open Terminal.</strong> Press <kbd>⌘</kbd> + <kbd>Space</kbd>, type <em>Terminal</em> and press Return. Paste this single line and press Return:<br><span class="c3d-cmd">curl -fsSL https://github.com/megatih/c3d-mcp/releases/latest/download/install.sh | bash</span></li>
  <li><strong>Answer the questions.</strong> The installer checks your Mac and tells you what it finds. If a helper program called Node.js is missing, it offers to install it for you. It always asks first, and it never asks for your password.</li>
  <li><strong>Allow the helper.</strong> While the installer runs, it opens <em>System Settings › Privacy &amp; Security</em> for you and waits. Switch on <strong>C3D Bridge Helper</strong> in the list (on the newest macOS the page is called <em>Device Control and Data Access</em>; on older versions it is <em>Accessibility</em>). This is what lets the AI press Cheetah3D's menu for you.</li>
  <li><strong>Restart Cheetah3D once.</strong> When the installer finishes, quit and reopen Cheetah3D so it notices the new bridge. You only ever need to do this once. (If the installer says it skipped its test picture, just run the same line again after restarting to confirm that everything works.)</li>
  <li><strong>Say hello to your AI.</strong> The installer connects the AI apps it finds on your Mac (it asks you first). Open one and try: <em>"Check that Cheetah3D is connected, then make a new scene with a red cube and render it."</em></li>
</ol>

<div class="c3d-card">
<p><strong>Want to read the installer first?</strong> Good idea! Download it with <span class="c3d-cmd">curl -fsSL https://github.com/megatih/c3d-mcp/releases/latest/download/install.sh -o install.sh</span>, open it in any text editor, then run it with <span class="c3d-cmd">bash install.sh</span>. You can also add <span class="c3d-cmd">--dry-run</span> to see what it <em>would</em> do without changing anything.</p>
<p><strong>If something goes wrong:</strong> the <a href="https://github.com/megatih/c3d-mcp/blob/main/docs/INSTALL.md">install guide</a> and the <a href="https://github.com/megatih/c3d-mcp/blob/main/docs/TROUBLESHOOTING.md">troubleshooting page</a> cover the common problems. macOS may also block the helper the very first time because it is not yet "notarized" by Apple; the install guide shows the one-line fix.</p>
</div>

## Update, repair or remove it later

You do not need to remember anything special. **Run the same install line again** and the installer first looks at your Mac and tells you what it found: nothing yet (a fresh install), the current version, an older version, a half-finished install, or a copy that was set up by hand. Then it offers only the sensible choices:

<table class="c3d-table">
  <thead><tr><th>You want to</th><th>What to do</th></tr></thead>
  <tbody>
    <tr><td>Update</td><td>Run the install line again and pick <em>Update</em>. The helper program is replaced too, and if the new one does not start, the old one is put back automatically.</td></tr>
    <tr><td>Repair</td><td>Pick <em>Repair</em>. It fixes only what is missing or broken and leaves everything else alone.</td></tr>
    <tr><td>Start over</td><td>Pick <em>Reinstall</em>. It rewrites everything, but keeps your settings, backups and your own Cheetah3D scripts.</td></tr>
    <tr><td>Just look</td><td><span class="c3d-cmd">c3d-mcp status</span> shows what is installed and what to run next. Add <span class="c3d-cmd">--dry-run</span> to any action to preview it.</td></tr>
    <tr><td>Remove it</td><td>Pick <em>Uninstall</em> to remove the bridge and the helper, or <em>Uninstall everything</em> to also remove the skills, the AI app entries and the installer's own folder. It lists what will go and asks first. Your Cheetah3D scripts and backups are never touched.</td></tr>
  </tbody>
</table>

<div class="c3d-card">
<p><strong>One thing to expect after an update:</strong> the helper program is signed but not notarized by Apple, so macOS treats a new version as a new app and asks you to switch on <em>C3D Bridge Helper</em> in System Settings again. The installer tells you when that is needed and opens the right page.</p>
</div>

The installer also adds a set of **skills**: short guidebooks that teach your AI how to use Cheetah3D well. They are the reason the AI knows, for example, which way rotation works in Cheetah3D, or how to check a render before moving on.

## Benchmark 1: the Cornell Box

To find out whether this really works, I needed tests. The first one is a classic from the world of computer graphics: the **Cornell Box**. It is a simple room with one red wall, one green wall and a lamp in the ceiling. It looks easy, but it is a tough test of lighting, because the red and green walls should softly "bleed" colour onto everything near them.

I made it harder (call it the *Cornell Box Deluxe*) by adding a tall box with a marble ball, a hand-made gold vase on a wooden box, and a chrome ball and a glass ball on a checkerboard rug.

<figure class="c3d-fig">
  <img src="/assets/img/c3d-mcp/cornell-final-falcon.jpg" alt="Final render of the Cornell Box Deluxe made with Cheetah3D's Falcon renderer: a white room with a red left wall and green right wall, a marble ball on a tall white box, a gold vase on a wooden box, and chrome and glass balls on a checkerboard rug.">
  <figcaption>The final Cornell Box Deluxe, built through c3d-mcp and rendered with Cheetah3D's <strong>Falcon</strong> renderer, with reflective and refractive caustics switched on. Look for the red and green light bouncing onto the white surfaces, the checkerboard reflected in the chrome ball and seen upside down through the glass ball, and the light refracting through the glass ball into its shadow.</figcaption>
</figure>

The AI worked in stages and looked at a rendered picture after every one, just as a person would:

<figure class="c3d-fig">
  <img src="/assets/img/c3d-mcp/cornell-steps.jpg" alt="Four stage images: an empty room with a ceiling lamp; the room with boxes, balls and a vase in plain grey; the same scene with colours and textures; and the final look with realistic light bounce.">
  <figcaption>How it came together: (1) the room, lamp and camera; (2) the objects, including a vase the AI modelled by writing a short script; (3) colours, wood, marble, chrome, glass and gold; (4) realistic light bounce switched on. These four step pictures use Cheetah3D's classic renderer; the final image above uses the Falcon renderer.</figcaption>
</figure>

This test also taught me something. The first attempt tilted the boxes the wrong way, because Cheetah3D measures rotation in a way the AI had guessed wrongly. We found it, fixed it, and wrote the lesson into the skills so no AI will make the same mistake again.

## Benchmark 2: the Cyberpunk Diorama

The second test is much bigger, and it is my favourite. I came across a video by **Muska** on YouTube, [*"GPT-6 Astra vs Claude Opus 5.5 – Cyberpunk Anime-Style 3D Modeling Challenge Timelapse"*](https://www.youtube.com/watch?v=SQs27US4FeI). In it, two AI models are challenged to recreate a detailed, anime-style cyberpunk Japanese building in Blender, using Blender MCP and a long, carefully written prompt.

<div class="c3d-card">
<p><strong>Credit where it is due.</strong> The challenge, the reference picture and the original prompt come from Muska's video and its accompanying document. I adapted that prompt so it works with Cheetah3D and c3d-mcp (for example, by removing the Blender-only features), and ran it with Claude Opus 5.5. Please go and watch the <a href="https://www.youtube.com/watch?v=SQs27US4FeI">original video</a> and visit <a href="https://www.youtube.com/@Muska-2026">Muska's channel</a>.</p>
</div>

Here is the original reference picture the AIs had to match, and the result the Blender MCP version produced in the video:

<div class="c3d-pair">
  <figure class="c3d-fig" style="flex: 858 1 0">
    <img src="/assets/img/c3d-mcp/cyberpunk-reference-crop.jpg" alt="The original reference picture: a detailed anime-style purple cyberpunk Japanese building with glowing orange windows, neon signs, pipes and plants.">
    <figcaption>The original reference picture from Muska's challenge (cropped to the building). Image credit: Muska (<a href="https://www.youtube.com/watch?v=SQs27US4FeI">video</a>).</figcaption>
  </figure>
  <figure class="c3d-fig" style="flex: 727 1 0">
    <img src="/assets/img/c3d-mcp/cyberpunk-blender-crop.jpg" alt="The Blender MCP result shown in the video: the cyberpunk building recreated in Blender by Claude Opus 5.5.">
    <figcaption>The Blender MCP result shown in the video (Claude Opus 5.5), cropped to the building. Image credit: Muska (<a href="https://www.youtube.com/watch?v=SQs27US4FeI">video</a>).</figcaption>
  </figure>
</div>

And here are all three together, with what Cheetah3D produced on the right:

<figure class="c3d-fig">
  <img src="/assets/img/c3d-mcp/cyberpunk-comparison.jpg" alt="Three images side by side: the original reference picture of a purple cyberpunk building, the Blender MCP result from the video, and the Cheetah3D result made with c3d-mcp.">
  <figcaption>Left: the reference picture from the challenge. Middle: the Blender MCP result shown in Muska's video (Claude Opus 5.5). Right: the Cheetah3D result made with c3d-mcp (also Claude Opus 5.5). Reference and Blender images are credited to Muska and shown here for comparison.</figcaption>
</figure>

### How we got there

The AI did not build it in one go. We followed the same steps a human 3D artist would, in eight stages, with a render after each one and a checkpoint saved so we could always go back:

<figure class="c3d-fig">
  <img src="/assets/img/c3d-mcp/cyberpunk-wip.jpg" alt="Eight work-in-progress renders, from plain lavender blocks through walls, storefronts, mechanical details, props and plants, materials, and finally lighting.">
  <figcaption>Selected work-in-progress renders: matching the camera, blocking out the volumes, adding walls and panels, storefronts and stairs, fans and pipes, paving and plants, layered materials, and finally lights and glow.</figcaption>
</figure>

After each stage the AI compared its picture with the reference, listed what was different, and fixed it before moving on. Along the way it made 29 test renders and used well over a hundred of c3d-mcp's tools. A few moments stood out for me:

- It noticed on its own that an awning sloped the wrong way, and corrected it.
- Cheetah3D crashed once. Because of the automatic checkpoints, the AI picked up from the last saved stage and carried on, and afterwards we traced the crash to one specific action and made c3d-mcp refuse to do it.
- The finished scene has **over 1,100 separate objects and 67 materials**, and the AI built it in roughly half an hour.

### The final result, and how amazed I was

<figure class="c3d-fig">
  <img src="/assets/img/c3d-mcp/cyberpunk-cheetah-final.jpg" alt="The final Cheetah3D render of the cyberpunk building: a purple three-storey building with glowing orange windows, a pink neon sign, an orange awning, stairs, pipes, plants and a paved base.">
  <figcaption>The final Cheetah3D render, 1456 × 816 pixels, rendered in a few seconds.</figcaption>
</figure>

I will be honest: **I was blown away.** I had pictured an AI placing a few boxes. Instead I watched a recognisable copy of that building appear in my favourite 3D app, with the same shape, the same colours, the same camera angle, the glowing windows, the neon sign, the pipes, the plants and the paving, all from words alone. It is not as polished as the Blender version in the video, which uses painterly shading and glow effects that Cheetah3D does not offer in the same way. But the fact that it works at all, in the app I have loved for years, made my day.

And here is the finished scene opened in Cheetah3D itself, so you can see it really is a normal, editable Cheetah3D document:

<figure class="c3d-fig">
  <img src="/assets/img/c3d-mcp/cheetah-final-scene.jpg" alt="Screenshot of the Cheetah3D window with the finished cyberpunk building in the 3D view, the materials at the bottom and the list of objects on the right.">
  <figcaption>The finished scene loaded in Cheetah3D: a normal document you can open, edit, re-light and render yourself.</figcaption>
</figure>

## Try it yourself

Once everything is installed, here are three prompts to get you started:

1. *"Create a new Cheetah3D document, build a simple table with four legs and a wood material, light it, and render it."*
2. *"Look at my current scene and tell me which objects have no material, then give them sensible ones."*
3. *"Add a three-point lighting setup and render a preview. If it looks too dark, fix it."*

<div class="c3d-btns">
  <a class="btn btn-primary btn-lg" href="https://github.com/megatih/c3d-mcp">The project on GitHub</a>
  <a class="btn btn-outline-primary btn-lg" href="https://github.com/megatih/c3d-mcp/releases/latest">Download the latest release</a>
  <a class="btn btn-outline-primary btn-lg" href="https://github.com/megatih/c3d-mcp/blob/main/docs/INSTALL.md">Install guide</a>
</div>

## Thank you, and let me know what you think

I hope you find c3d-mcp useful, and that it makes Cheetah3D even more fun for you the way it has for me. This is a young project, and I would love to hear how it goes on your Mac: what worked, what confused you, what you would like it to do next.

- **Questions and ideas:** [start a conversation on GitHub Discussions](https://github.com/megatih/c3d-mcp/discussions), or leave a comment below (you will need a free GitHub account, which keeps spam away).
- **Found a bug?** Please [open an issue](https://github.com/megatih/c3d-mcp/issues).

### Credits

- **Cheetah3D** is created by **Martin Wengenmayer**, an independent developer who has been building and refining it since the early 2000s. Thank you, Martin, for making such an amazing app: friendly, fast, and a joy to use. I sincerely hope Cheetah3D will continue to be supported, developed and improved well into the future. If you use and love it too, please support it by [buying a licence from the official Cheetah3D website](https://www.cheetah3d.com).
- **Muska**, for the [video and challenge](https://www.youtube.com/watch?v=SQs27US4FeI) that inspired the Cyberpunk Diorama test, and for the reference image and prompt it was based on.
- **Tonio Loewald**, whose [c3d-scripting-kb](https://github.com/tonioloewald/c3d-scripting-kb) (the Cheetah3D API reference, example scripts, linter rules and forum-derived gotchas, collected from the posts of the Cheetah3D forum community) and online book [Learn 3D with Cheetah 3D](https://learn3d.loewald.com) taught c3d-mcp a lot: it uses them for its documentation search, script linting and agent skills. Everything I took from them was tested against Cheetah3D 8.1.3 first, and where the app behaved differently, the correction is mine, not theirs. Thank you!
- The AI assistants used to build and test this project, and the open **Model Context Protocol** that makes it all possible.

*c3d-mcp is an independent, community project. It is not made by, affiliated with or endorsed by the makers of Cheetah3D.*
