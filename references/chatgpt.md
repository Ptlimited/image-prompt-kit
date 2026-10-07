# Prompting ChatGPT Images

Last checked: 2026-10-07, against OpenAI's own docs. Links at the bottom.

## How it likes to be asked

- **Lead with the result:** what it is, what it's for, the framing and the shape.
- **Then fill in 4 parts:** the scene, the subject, the details, the limits. OpenAI's guide uses this order. Short paragraphs, labeled lines and lists each work.
- **Spell out the limits.** Unlike Google's advice, OpenAI's guide says to name what to leave out: "no extra text", "no watermark", "no logos", "do not add new elements".
- **For a real photo look, say "real photograph".** OpenAI's guide treats lens and camera words as hints for the look, so lean on plain words about light and materials.
- **For a natural photo,** skip "cinematic lighting" and heavy color grading.

## Text in the image

- Put the exact words in quotes and say where they sit and how they look ("small white capitals along the bottom").
- Spell an unusual word letter by letter.
- Add "no extra text" so it doesn't invent captions.

## Photos of a person or product

- Attach the photo and give it a job: "Image 1 is the person. Image 2 is the style to match."
- Say what stays: "Keep their face exactly the same."

## Settings in ChatGPT

- **Thinking effort:** High for detailed scenes and lettering. Lower for quick drafts.
- **Aspect ratio:** pick it if the shape option shows, and write it at the end of the prompt too.

## Editing

1 change per message. Say "Change only the background to a beach. Keep the person, pose and lighting the same." If later edits start to drift, repeat what has to stay.

## Sources

- OpenAI image prompting guide: https://developers.openai.com/api/docs/guides/image-prompting
- OpenAI image generation guide: https://developers.openai.com/api/docs/guides/image-generation
- Introducing ChatGPT Images 2.5: https://openai.com/index/introducing-chatgpt-images-2-5/
