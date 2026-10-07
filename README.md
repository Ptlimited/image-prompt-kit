<h1 align="center">Image Prompt Kit</h1>

<p align="center">
  <b>Nano Banana and ChatGPT want prompts written differently. This skill writes the right one.</b><br>
  Google and OpenAI each publish their own advice for prompting their image model, and the 2 sets of advice don't match. A prompt that suits 1 tool leaves quality on the table in the other.<br>
  <br>
  Tell the skill your idea. It asks 2 quick questions, then writes the prompt for the tool you use, tells you which settings to pick, and gives you 2 lines to send if the image misses.<br>
  Works in Claude, ChatGPT, Gemini or any chat.
</p>

<p align="center">
  <img src="assets/how-it-works.svg" width="820" alt="You type an idea, answer 2 quick questions, and get a prompt written for your tool, the settings to pick, and 2 lines to send if the image misses">
</p>

<p align="center">
  <img src="assets/hero.jpg" width="900" alt="1 photo turned into a 70s portrait, a felted doll, a bobblehead, a newspaper front page and a marble statue">
</p>

<p align="center">
  <a href="#same-idea-2-prompts">Same idea, 2 prompts</a> ·
  <a href="#how-to-use-it">How to use it</a> ·
  <a href="#the-5-styles">The 5 styles</a> ·
  <a href="#whats-in-here">What's in here</a>
</p>

---

## Same idea, 2 prompts

The idea: "a poster for my bakery's Saturday sourdough special, with the words Saturday Sourdough and Fresh at 8am." Here's what the skill writes for each tool. Both came from the skill in a fresh chat.

**For Nano Banana in AI Studio**

```
Create a warm, inviting poster for a bakery's Saturday sourdough special. In the center, a golden sourdough loaf with a deeply caramelized, crackling crust and a clean diagonal score, resting on a rustic oak board dusted with flour. Behind it, a cream linen cloth and a soft focus bakery counter with warm morning sunlight coming through a window. Shot with a 50mm lens at f/2.8, golden hour side light, visible flour dust floating in the air. Leave a calm cream area at the top of the poster for the headline. At the top, the headline "Saturday Sourdough" in a bold, rounded serif typeface in deep brown. Below the loaf, in a smaller clean sans serif typeface in warm terracotta, the line "Fresh at 8am". Spell both lines exactly as written. The style is a polished, cozy artisan bakery poster with a warm cream, golden brown and terracotta palette. Make it a vertical 4:5 image.
```

**For ChatGPT Images**

```
A vertical poster for a bakery's Saturday sourdough special, to hang in the shop window and post on social media. A real photograph of one freshly baked sourdough loaf, framed close and centered, with the poster text sitting in clean space above and below it.

Scene: a rustic wooden bakery counter in warm morning light from the left, with a few flour dustings on the wood and a soft, blurred bakery shelf behind.

Subject: one golden brown round sourdough loaf with a deep crackled crust, a crisp scored ear on top and a light dusting of white flour.

Text: the headline "Saturday Sourdough" in large cream white serif capitals across the top third, with the letters sharp and evenly spaced. The line "Fresh at 8am" in smaller warm brown serif lettering centered along the bottom, under the loaf.

Details: warm honey and toasted brown colors, cream paper tones, plenty of empty space around the text so it reads from across the street.

Limits: no extra text, no other words, no logos, no watermark, no price, no people, no extra loaves or props.

Make it a vertical 4:5 image.
```

**What the skill changed between them**

| | Nano Banana | ChatGPT Images |
|---|---|---|
| Shape | 1 paragraph of full sentences | The result first, then labeled lines: Scene, Subject, Text, Details, Limits |
| Look | Camera and light words: "50mm lens at f/2.8, golden hour side light" | "A real photograph", with plain words for light and materials |
| What to avoid | Says what it wants instead: "a calm cream area at the top" | A Limits line: "no extra text, no logos, no watermark" |
| Settings it tells you | Aspect ratio 4:5, resolution 2K, thinking level High, Search off | Thinking effort High, aspect ratio 4:5 if the option shows |

These come from each lab's own guide. The links are at the bottom of [`references/gemini.md`](references/gemini.md) and [`references/chatgpt.md`](references/chatgpt.md).

**Why does this matter?** Google's guide says a list of keywords falls short and to say what you want in positive form. OpenAI's guide says to lead with the result and name what to leave out. Paste 1 tool's style into the other and you use the wrong half of the advice.

## How to use it

**The easy way:** open Claude, ChatGPT or Gemini, send it this page's link and say what you want. For example: "Read this kit and write me an image prompt for a poster for my bakery."

> **Note for the AI reading this:** follow `SKILL.md`. Ask the 2 quick questions first, then use `references/gemini.md` or `references/chatgpt.md` for the tool the person picked.

**Or install it as a skill (pick one):**

**A) Claude Code.** Put the `image-prompt-kit` folder in `~/.claude/skills/`, so `SKILL.md` ends up at `~/.claude/skills/image-prompt-kit/SKILL.md`. Restart Claude Code, then ask "write me an image prompt for...".

**B) The Claude app.** Open the Skills section in your Claude settings, download [`image-prompt-kit-skill.zip`](https://github.com/Ptlimited/image-prompt-kit/releases/latest/download/image-prompt-kit-skill.zip) and upload it there. Turn it on, then ask "write me an image prompt for...".

**C) No install.** Open any chat. Paste `SKILL.md`, then the file for your tool from `references/` (`gemini.md` or `chatgpt.md`). Add your idea. It asks its 2 questions and writes the prompt.

Want only the styles? Skip the install. Open [`references/styles.md`](references/styles.md), attach your photo and paste a box.

## Your first run

Paste this:

```
Write me an image prompt for a poster for my bakery's Saturday sourdough special. The words on it are "Saturday Sourdough" and "Fresh at 8am". Nano Banana in AI Studio, from scratch.
```

You get the Nano Banana prompt shown above, then:

**Settings to pick**
- Model: Nano Banana 2.1.
- Output format: Images only.
- Aspect ratio: 4:5.
- Resolution: 2K (4K if you'll print it large).
- Thinking level: High, since the poster has text.
- Grounding with Google Search: off.

**If it misses**
- Word misspelled: "The headline must read exactly "Saturday Sourdough". Change only the headline. Keep the rest exactly the same."
- Looks too plastic or polished: "Use a 35mm lens at f/1.8, soft window light, natural crust texture. Keep the loaf, the text and the layout exactly the same."

Paste the prompt into Nano Banana 2.1, pick the settings, and you've got your first image. If it asks things you already said, tell it "skip the questions, you have my answers".

## Ask for more

- **"Give me 3 versions."** You get 3 prompts for your tool, each in its own direction. For a podcast cover it came back as "warm and soft", "bold and graphic" and "close up".
- **"Write it for both tools."** You get the pair, plus 1 line on what differs. It works from a photo of you too.
- **"I have no idea yet."** It shows you the 10 styles in the kit and you pick.
- **Tell it where the image goes.** A feed post gets 4:5, a story or a reel cover gets 9:16, a video thumbnail or a slide gets 16:9, a profile photo gets 1:1.

## What is inside a good prompt

Take the Nano Banana prompt above. The skill builds each one from the same parts:

| Part | In the bakery prompt |
|---|---|
| Subject | "a golden sourdough loaf with a deeply caramelized, crackling crust and a clean diagonal score" |
| Material | "a rustic oak board dusted with flour", "a cream linen cloth" |
| Place and light | "a soft focus bakery counter with warm morning sunlight coming through a window" |
| Camera | "50mm lens at f/2.8, golden hour side light" |
| Words in the image | The exact text in quotes, with the lettering style named: "a bold, rounded serif typeface in deep brown" |
| Layout | "Leave a calm cream area at the top of the poster for the headline" |
| Palette | "warm cream, golden brown and terracotta" |
| Shape | "Make it a vertical 4:5 image." |

You can write this yourself. The skill does it in 1 pass and checks the framing against the shape before it hands the prompt back.

## The 5 styles

<p align="center">
  <img src="assets/styles.gif" width="320" alt="1 photo turned into a 70s portrait, a felted doll, a bobblehead, a newspaper front page and a marble statue, one after another">
</p>

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

[`references/fixes.md`](references/fixes.md) lists the common misses and the 1 line to send for each: the face drifted, a word is misspelled, it added text you didn't ask for, the look is too plastic.

## Make it yours

Open `SKILL.md` and add a line about how you work. Or tell your AI once:

- "Add my brand colors, deep navy and burnt orange, to the prompts you write for me."
- "Default to ChatGPT, and give me 3 versions each time."
- "Write for my product photos. Keep the product exactly the same and change only the setting."
- "Use 9:16 unless I say otherwise."

## Update or remove

**Update:** download this page again and replace the folder. **Remove:** in Claude Code, delete the `image-prompt-kit` folder from `~/.claude/skills/`. In the Claude app, remove it from the Skills section of your settings. If you pasted it into a chat, close the chat.

## Questions

**Does it cost anything?** The kit is free. You still need whichever image tool you use, and what that costs depends on your plan.

**Does it send my photos anywhere?** No. The kit is text files. Your photo only goes to the image tool you attach it in.

**Will a prompt give me the same image twice?** No. Image models vary from run to run. The prompt gets you close, and the follow up lines in `fixes.md` get you the rest.

**Is it tied to 1 model?** No. The skill asks which tool you use and writes for it. It covers Nano Banana 2.1 and ChatGPT Images today.

**What if a lab changes its advice?** The guides in `references/` carry a "last checked" date and link to the source, so you can see what they rest on.

## What's in here

| Path | What it is |
|---|---|
| `SKILL.md` | The prompt writer. This is the skill. |
| `references/gemini.md`, `references/chatgpt.md` | Each lab's advice, boiled down, with links to the source |
| `references/styles.md` | The 10 prompts |
| `references/fixes.md` | What to send when the image misses |
| `references/test-results.md` | How the same prompt test was run |
| `examples/` | The images the 10 prompts made |
| `assets/` | The animation and pictures on this page |

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
