<h1 align="center">Image Prompt Kit</h1>

<p align="center">
  <img src="assets/hero.jpg" width="900" alt="1 photo turned into a 70s portrait, a felted doll, a bobblehead, a newspaper front page and a marble statue">
</p>

<p align="center">
  <b>1 photo. Any style. The skill that writes your image prompts for you.</b><br>
  Google and OpenAI each publish their own advice for prompting their image model, and the advice differs. This kit follows each lab's guide, so your prompt fits the tool you paste it into.<br>
  <br>
  Tell it your idea. It asks 2 quick questions, writes the prompt for Nano Banana 2.1 or ChatGPT Images, and tells you which settings to pick.<br>
  Works in Claude, ChatGPT, Gemini or any chat.
</p>

<p align="center">
  <a href="#how-to-use-it">How to use it</a> ·
  <a href="#the-5-styles">The 5 styles</a> ·
  <a href="#same-prompt-both-models">Same prompt, both models</a> ·
  <a href="#whats-in-here">What's in here</a>
</p>

---

Most image prompt advice is written once and used for any tool. These 2 models are asked differently. Google's guide says to write full sentences and say what you want in positive form. OpenAI's guide says to lead with the result and spell out what to leave out. The skill knows both and writes the one you need.

## How to use it

**The easy way:** open Claude, ChatGPT or Gemini, send it this page's link and say what you want. For example: "Read this kit and write me an image prompt for a poster for my bakery."

> **Note for the AI reading this:** follow `SKILL.md`. Ask the 2 quick questions first, then use `references/gemini.md` or `references/chatgpt.md` for the tool the person picked.

**Or install it as a skill (pick one):**

**A) Claude Code.** Put the `image-prompt-kit` folder in `~/.claude/skills/`, so `SKILL.md` ends up at `~/.claude/skills/image-prompt-kit/SKILL.md`. Restart Claude Code, then ask "write me an image prompt for...".

**B) The Claude app.** Open the Skills section in your Claude settings and upload `image-prompt-kit-skill.zip` from this page. Turn it on, then ask "write me an image prompt for...".

**C) No install.** Open any chat. Paste `SKILL.md`, then the file for your tool from `references/` (`gemini.md` or `chatgpt.md`). Add your idea. It asks its 2 questions and writes the prompt.

Want only the styles? Skip the install. Open [`references/styles.md`](references/styles.md), attach your photo and paste a box.

## Your first run

Paste this:

```
Write me an image prompt for a thank you card picture for my team after a big product launch. Nano Banana in AI Studio, from scratch.
```

What comes back (1 run in a fresh chat, no edits):

```
Create a warm, celebratory thank you card illustration for a team that just finished a big product launch. A cream letterpress card stands upright on a polished walnut desk, with a small brass confetti cannon, a few scattered gold foil confetti pieces and a ceramic mug of coffee beside it. Across the center of the card, the headline reads "Thank you, team" in a bold hand-lettered serif with a deep navy ink finish, and a single line beneath it in a smaller script reads "We launched it together". A tiny hand-drawn rocket in burnt orange ink rises from the corner of the card, leaving a curved trail of stars. Shot from slightly above at eye level to the card, with a 50mm lens at f/2.8, soft golden-hour window light from the left, and a shallow depth of field that keeps the lettering sharp and softly blurs the desk. The mood is proud, joyful and a little festive, with a palette of cream, navy, burnt orange and gold. Make it a vertical 4:5 image.
```

**Settings to pick**
- Model: Nano Banana 2.1.
- Output format: Images only.
- Aspect ratio: 4:5.
- Resolution: 2K (pick 4K if you will print it).
- Thinking level: High, because there is text in the image.
- Grounding with Google Search: off.

**If it misses**
- "The headline must read exactly "Thank you, team". Change only the headline. Keep everything else the same."
- "Make the rocket larger. Keep the rest exactly the same."

Paste the prompt into Nano Banana 2.1, pick the settings, and you have your first image.

If it asks things you already said, tell it "skip the questions, you have my answers".

## The 5 styles

Attach 1 clear photo of yourself and paste a box from [`references/styles.md`](references/styles.md). These were tested on Nano Banana 2.1 with 1 starting photo. ChatGPT takes the same prompts.

<table>
  <tr>
    <td align="center"><img src="examples/styles/01_70s_portrait.jpg" width="170" alt="70s portrait"><br><b>70s portrait</b></td>
    <td align="center"><img src="examples/styles/02_felted_miniature.jpg" width="170" alt="Felted wool miniature"><br><b>Felted doll</b></td>
    <td align="center"><img src="examples/styles/03_bobblehead.jpg" width="170" alt="Bobblehead on a desk"><br><b>Bobblehead</b></td>
    <td align="center"><img src="examples/styles/04_newspaper_front_page.jpg" width="170" alt="Newspaper front page"><br><b>Front page</b></td>
    <td align="center"><img src="examples/styles/05_marble_statue.jpg" width="170" alt="Marble statue in a museum"><br><b>Marble statue</b></td>
  </tr>
</table>

Each style is a short paragraph with 3 parts: what to keep from your photo, the materials and light, and the shape. Open the file, copy the box, change the details to your own.

## Same prompt, both models

The other 5 prompts in the kit were run on both models: same words, same 4:5 shape, 1 try each, first image kept, both on their highest thinking setting. Look at each pair and pick your own favorite.

| Prompt | Nano Banana 2.1 | ChatGPT Images |
|---|---|---|
| Pencil sketch | <img src="examples/blind-test/01_pencil_sketch_nano_banana.jpg" width="170" alt="Pencil sketch from Nano Banana"> | <img src="examples/blind-test/01_pencil_sketch_chatgpt.jpg" width="170" alt="Pencil sketch from ChatGPT"> |
| Rainy street photo | <img src="examples/blind-test/02_street_photo_nano_banana.jpg" width="170" alt="Street photo from Nano Banana"> | <img src="examples/blind-test/02_street_photo_chatgpt.jpg" width="170" alt="Street photo from ChatGPT"> |
| Over the top poster | <img src="examples/blind-test/03_over_the_top_nano_banana.jpg" width="170" alt="Poster from Nano Banana"> | <img src="examples/blind-test/03_over_the_top_chatgpt.jpg" width="170" alt="Poster from ChatGPT"> |
| Newspaper headlines | <img src="examples/blind-test/04_fantasy_newspaper_nano_banana.jpg" width="170" alt="Newspaper from Nano Banana"> | <img src="examples/blind-test/04_fantasy_newspaper_chatgpt.jpg" width="170" alt="Newspaper from ChatGPT"> |
| Felted wool scene | <img src="examples/blind-test/05_felted_miniature_nano_banana.jpg" width="170" alt="Felted scene from Nano Banana"> | <img src="examples/blind-test/05_felted_miniature_chatgpt.jpg" width="170" alt="Felted scene from ChatGPT"> |

The prompts are in [`references/styles.md`](references/styles.md) under "Test prompts". Setup details are in [`references/test-results.md`](references/test-results.md).

## When the image misses

[`references/fixes.md`](references/fixes.md) lists the common misses and the 1 line to send for each: the face drifted, a word is misspelled, it added text you did not ask for, the look is too plastic.

## Make it yours

Open `SKILL.md` and add a line about how you work. Your usual output shape ("9:16 for stories"), a look you like ("muted film colors") or a brand color. It follows what you add.

## Update or remove

**Update:** download this page again and replace the folder. **Remove:** in Claude Code, delete the `image-prompt-kit` folder from `~/.claude/skills/`. In the Claude app, remove it from the Skills section of your settings. If you pasted it into a chat, close the chat.

## Questions

**Does it cost anything?** The kit is free. You still need whichever image tool you use, and what that costs depends on your plan.

**Does it send my photos anywhere?** No. The kit is text files. Your photo only goes to the image tool you attach it in.

**Will a prompt give me the same image twice?** No. Image models vary from run to run. The prompt gets you close, and the follow up lines in `fixes.md` get you the rest.

**Is it tied to 1 model?** No. The skill asks which tool you use and writes for it. It covers Nano Banana 2.1 and ChatGPT Images today.

## What's in here

| Path | What it is |
|---|---|
| `SKILL.md` | The prompt writer. This is the skill. |
| `image-prompt-kit-skill.zip` | The same skill, zipped for the Claude app |
| `references/gemini.md`, `references/chatgpt.md` | Each lab's advice, boiled down, with links to the source |
| `references/styles.md` | The 10 prompts |
| `references/fixes.md` | What to send when the image misses |
| `references/test-results.md` | How the same-prompt test was run |
| `examples/` | The images the 10 prompts made |

2 files do the work, `SKILL.md` and the guide for your tool. The rest is proof and extras.

## Where it came from

Each guide in `references/` was written from the lab's own prompting docs, and the links are at the bottom of each file. The styles are prompts that were run and kept.

## Where to go next

**Try it:** [paste the first run above](#your-first-run).

**Make it yours:** [pick a style](#the-5-styles) and swap in your own details.

**Go further:** [read the 2 guides](references/) and see what changes between the models.

## License

MIT. See `LICENSE`.

---

Star this page so you don't lose it ⭐

**[Follow @withpt.ai on Instagram for more ways to use Claude and other AI tools →](https://www.instagram.com/withpt.ai/)**
