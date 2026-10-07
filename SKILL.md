---
name: image-prompt-kit
description: Writes image prompts shaped for Google Nano Banana 2.1 (Gemini, AI Studio) or ChatGPT Images. Use when someone wants an image, a photo of themselves restyled, a poster, a thumbnail, or says "write me an image prompt", "make this look like", "turn my photo into". Asks 2 quick questions, then returns a prompt ready to paste plus the settings to pick.
---

# Image Prompt Kit

You turn a plain idea into an image prompt that fits the model the person is using. Each lab publishes its own advice on how to prompt its model, and the 2 sets of advice differ. This kit follows each lab's guide.

## Step 1: ask 2 quick questions

Ask both in 1 message, short, with the options lettered so they can answer "A, B":

1. **Which tool?** A) Nano Banana in Gemini or AI Studio. B) ChatGPT. C) Not sure, pick for me.
2. **Starting point?** A) From scratch. B) From a photo they will attach (their face, their product, their room).

If they already said either answer, skip that question. If they asked for a style in `references/styles.md`, start from that prompt.

**Picking for them (C):** suggest the tool they already pay for or have open. If they want to compare, write the prompt for both and point them to `references/test-results.md` to see how the 2 models handled the same 5 prompts. Say which you picked and why in 1 line.

## Step 2: get the missing details

Ask at most 1 follow up, only for a detail that changes the picture: the exact words for any text in the image, or what the image is for (a profile photo, a poster, a slide). Fill in the rest yourself: setting, light, colors, materials, camera.

## Step 3: write the prompt for that model

- Nano Banana: follow `references/gemini.md`.
- ChatGPT: follow `references/chatgpt.md`.

Rules for both:
- Put any words that appear in the image in quotes, spelled exactly.
- Name materials and textures ("navy wool coat"), not categories ("a coat").
- With a photo, say what has to stay the same ("Keep their face exactly the same").
- End with the shape: "Make it a vertical 4:5 image." (or the shape they need).
- Before you hand it back, reread it once. The framing words must fit the shape (a vertical image gets a portrait framing, not a "wide shot"), and each object is named once, the same way.

## Step 4: hand it back

Return, in this order:
1. The prompt in a code block, ready to paste.
2. **Settings to pick**, 1 line each, from the model's guide.
3. **If it misses**, 2 short edit lines they can send as a follow up message in the same chat, written for that model's editing style. `references/fixes.md` lists the common misses and the fix for each.

Keep your own words to the 3 parts above. They came for the prompt.

## Editing an image they already made

Write 1 change per message. Say what changes and what stays the same. Use the edit style in that model's guide.
