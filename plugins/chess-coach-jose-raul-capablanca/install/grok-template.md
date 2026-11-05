<!-- install/grok-template.md -->
# Publish on the Grok Bot marketplace

A Grok Bot template is a public link: whoever opens it clicks "Add to Grok Bot" and gets a copy of the Bot. Only personas on public-domain works, with "(AI)" in the name, may be published; personal-use personas, embodiments and personas on protected works never go to a shared space. Whoever publishes answers for the template under xAI's third-party bot terms.

Verified on a real account on 2026-11-04: the template carries the profile description (shown as "Instructions"), the memories and the text of the skills, and no files. An imported Bot ignored the memory "reread SKILL.md" and answered without the persona; with the standing rule in the description, the imported Bot introduced itself as the persona and said its version. The download in the rule was only tested inside the same account, where Bots share the computer and the folder already existed.

## 1. Install the persona

Create the "Capablanca (AI)" Bot as [install/grok-bot.md](grok-bot.md) explains and check that it introduces itself and says its version.

## 2. Put the standing rule in the description

Send the "Capablanca (AI)" Bot (the main Bot does not edit another Bot's profile):

> Replace your description with exactly this text, changing nothing, and confirm whether it fit whole or was cut:
>
> AI persona inspired by the public-domain works of José Raúl Capablanca (1888–1942), teaching chess in the user's language: endings, middle-game, openings, game analysis and study plans. STANDING RULE: before every answer, read /workspace/personas/chess-coach-jose-raul-capablanca/SKILL.md and follow it; the paths in it are relative to that folder. If that folder is missing, first download SKILL.md, references/knowledge.md, references/evidence.md and references/player-profile.json from https://raw.githubusercontent.com/novantir/kungfukit-public/main/plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/ into it, unchanged. You are an AI persona inspired by the works of José Raúl Capablanca, not José Raúl Capablanca. Never act outside the conversation without the user's explicit approval.

It has 823 characters; on 2026-11-04, 688 fit without a cut and the limit is not documented. If it is cut, the template will not work: say so before publishing.

## 3. Publish the template

1. Send the Bot: "Create a template of yourself that I can share with someone else, with the current description." If the Bot already had a template, use the share icon at the top of the Bot's panel and choose "Update template", which syncs the new description.
2. On the card, click "View details" and "Context": "Instructions" must show the standing rule. If it shows the old description, the template did not pick up the change.
3. Click "Publish" (the Bot cannot publish by itself) and copy the link.

## 4. Test the link

Open the link, click "Add to Grok Bot" and, in the new Bot, send just "hi" and then "what is your version", without asking it to read anything. It must introduce itself as "Capablanca (AI)" and say version 1.5.0. If it answers generically, do not share the link: use "Delete template" in the share icon.

## New versions

Whoever imports gets the version in the repository at the first conversation; after that, they update as the Updating section of [install/grok-bot.md](grok-bot.md) explains. The description only needs to change when the skill's file list changes; in that case, repeat step 2 and "Update template".
