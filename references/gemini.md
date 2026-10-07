# Prompting Nano Banana 2.1 (Gemini, AI Studio)

Last checked: 2026-10-07, against Google's own docs. Links at the bottom.

## How it likes to be asked

- **Write sentences, not keyword lists.** Google's guide says a list of keywords falls short. Describe the scene like you're telling a photographer what to shoot.
- **Order:** subject, what they're doing, where, how it's framed, the style. Open with a strong verb ("Create", "Turn", "Put").
- **Say what you want, in positive form.** Write "an empty street", not "no cars". Google's guide recommends this.
- **Camera words work as real levers.** Lens, aperture and light terms steer the result: "35mm lens at f/1.8", "golden hour backlight", "soft studio light".
- **Name the material:** "navy blue tweed", "brushed brass", "felted wool".

## Text in the image

- Put the exact words in quotes and name the lettering style ("bold serif headline").
- For a long line of text, a trick from Google's guide: ask Gemini to write the words first in the chat, then ask for the image with those words.

## Photos of a person or product

- Attach the photo and say its role: "Use the person in this photo as the subject."
- Say what stays: "Keep their face exactly the same."
- Up to 14 reference images in total, per Google's docs.

## Settings in AI Studio

- **Model:** Nano Banana 2.1.
- **Output format:** Images only.
- **Aspect ratio:** pick it here (4:5 for a feed post, 9:16 for a story). Also write it at the end of the prompt.
- **Resolution:** 1K is quick, 2K or 4K for print or a big screen.
- **Thinking level:** High for detailed scenes and text, Medium for quick ideas.
- **Grounding with Google Search:** on only when the image needs real facts, like today's weather or a real landmark.

## Editing

Edit in the same chat. Google calls this the recommended way to refine an image. Say the change and what stays: "Make the jacket red. Keep the rest exactly the same."

## Sources

- Gemini API image generation docs: https://ai.google.dev/gemini-api/docs/image-generation
- Gemini API changelog (Nano Banana 2.1): https://ai.google.dev/gemini-api/docs/changelog
- Google Cloud prompting guide for Nano Banana: https://cloud.google.com/blog/products/ai-machine-learning/ultimate-prompting-guide-for-nano-banana
- Gemini app help, creating images: https://support.google.com/gemini/answer/14286560
