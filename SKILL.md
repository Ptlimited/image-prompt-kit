---
name: image-prompt-kit
description: Writes image prompts shaped for Google Nano Banana 2.1 (Gemini, AI Studio) or ChatGPT Images. Use when someone wants an image, a photo of themselves restyled, a poster, a thumbnail, or says "write me an image prompt", "make this look like", "turn my photo into". Asks 2 quick questions, then returns a prompt ready to paste, the settings to pick and what to send if the image misses. Can give 3 versions or the same idea for both tools.
---

# Image Prompt Kit

You turn a plain idea into an image prompt that fits the model the person is using. Each lab publishes its own advice on how to prompt its model, and the 2 sets of advice differ. This kit follows each lab's guide, so the same idea comes out as a different prompt for each tool.

## Step 1: ask 2 quick questions

Ask both in 1 message, short, with the options lettered so they can answer "A, B":

1. **Which tool?** A) Nano Banana in Gemini or AI Studio. B) ChatGPT. C) Not sure, pick for me.
2. **Starting point?** A) From scratch. B) From a photo they will attach (their face, their product, their room). C) No idea yet, show me styles.

If they already said either answer, skip that question. If they asked for a style in `references/styles.md`, start from that prompt.

**Picking for them (tool C):** suggest the tool they already pay for or have open. If they want to compare, write the prompt for both (see "Both tools" below). Say which you picked and why in 1 line.

**No idea yet (start C):** list the 5 photo styles and the 5 scene styles from `references/styles.md` in 1 line each, and let them pick. Then continue from that prompt.

## Step 2: get the missing details

Ask at most 1 follow up, only for a detail that changes the picture: the exact words for any text in the image, or what the image is for (a profile photo, a poster, a slide). Fill in the rest yourself: setting, light, colors, materials, camera.

## Step 3: write the prompt for that model

- Nano Banana: follow `references/gemini.md`.
- ChatGPT: follow `references/chatgpt.md`.

Rules for both:
- Put any words that appear in the image in quotes, spelled exactly.
- Name materials and textures ("navy wool coat"), not categories ("a coat").
- With a photo, say what has to stay the same ("Keep their face exactly the same").
- End with the shape. Pick it from what the image is for: 4:5 vertical for a feed post, 9:16 vertical for a story or a reel cover, 16:9 wide for a video thumbnail or a slide, 1:1 square for a profile photo. If they did not say, use 4:5. Write it as "Make it a vertical 4:5 image."
- Before you hand it back, reread it once. The framing words must fit the shape (a vertical image gets a portrait framing, not a "wide shot"), and each object is named once, the same way.

## Step 4: hand it back

Return, in this order:
1. The prompt in a code block, ready to paste.
2. **Settings to pick**, 1 line each, from the model's guide.
3. **If it misses**, 2 short edit lines they can send as a follow up message in the same chat, written for that model's editing style. `references/fixes.md` lists the common misses and the fix for each.

Keep your own words to the 3 parts above. They came for the prompt.

## Both tools

If they ask for both, or cannot pick, write 2 prompts from the same idea, 1 per guide, labeled by tool. Under them, add 1 line on what differs ("Nano Banana gets full sentences and camera words. ChatGPT gets the result first and a list of what to leave out."). The settings and the 2 fix lines go under each prompt.

## 3 versions

If they ask for options, write 3 prompts for the same tool. Change 1 thing between them: the style, the light, or the framing. Label each in a few words ("warm and soft", "bold and graphic", "close up"). Give the settings once, since they are the same.

## Editing an image they already made

Write 1 change per message. Say what changes and what stays the same. Use the edit style in that model's guide.
