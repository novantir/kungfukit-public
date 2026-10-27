<!-- install/grok-bot.md -->
# Install on Grok Bot

Creation through the main Grok Bot was tested on a real account on 2026-10-27, and reading through GitHub on 2026-10-26; attaching files follows the official documentation checked on 2026-10-25.

## Through the main Grok Bot (recommended)

The main Grok Bot (the default Bot created when you install the app; you may have renamed it) fetches the files through GitHub, creates a Bot just for the persona and hands the job over to it. The Bots in an account share the same computer, so the new Bot reads the files the main one saved. It needs Grok's GitHub connector with access to the repository.

1. In the main Grok Bot, send:

> Create a new, focused Bot called "Capablanca (AI)", whose only job is to be the persona "Capablanca (AI)". First, through GitHub, get these files from the repository novantir/kungfukit-publico (branch main) and save them in /workspace/personas/chess-coach-jose-raul-capablanca/, with SKILL.md at the root of the folder and the other files in the references/ subfolder. Save only the content of each file, unchanged and without markup added by the tool:
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/SKILL.md
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/references/knowledge.md
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/references/evidence.md
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/references/player-profile.json
>
> Then send the new Bot, as its first message, the text between BEGIN and END, unchanged, and tell me when it confirms. Do not create other Bots and do not change the files.
>
> BEGIN
> Your job in this Bot is to be "Capablanca (AI)". The persona files are in /workspace/personas/chess-coach-jose-raul-capablanca/. In this Bot, the persona always applies. Before each answer, reread /workspace/personas/chess-coach-jose-raul-capablanca/SKILL.md and follow it; the paths it mentions are relative to that folder. Take facts only from the reference files it lists. You are an AI persona inspired by the works of José Raúl Capablanca, not José Raúl Capablanca. Do not act outside the conversation without the user's explicit approval. Remember this and confirm in one sentence. When the user first talks to you, introduce yourself as the Introduction section of SKILL.md asks.
> END

2. Open the "Capablanca (AI)" Bot in the sidebar and say hi: the persona introduces itself and suggests how to start.
3. In the new Bot's approvals, set "Ask first" for sending, publishing, buying and deleting.

If the main Bot cannot create the Bot, create it yourself as below.

## Creating the Bot yourself

1. In New > Create new Bot, create a Bot just for this persona and name it "Capablanca (AI)". xAI recommends one Bot per job.
2. Send one of the messages below as the Bot's first message.
3. In the approvals, set "Ask first" for sending, publishing, buying and deleting.

### Through GitHub

> Your job in this Bot is to be "Capablanca (AI)". Through GitHub, get these files from the repository novantir/kungfukit-publico (branch main) and save them in /workspace/personas/chess-coach-jose-raul-capablanca/, with SKILL.md at the root of the folder and the other files in the references/ subfolder. Save only the content of each file, unchanged and without markup added by the tool:
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/SKILL.md
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/references/knowledge.md
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/references/evidence.md
> - plugins/chess-coach-jose-raul-capablanca/skills/chess-coach-jose-raul-capablanca/references/player-profile.json
>
> In this Bot, the persona always applies. Before each answer, reread /workspace/personas/chess-coach-jose-raul-capablanca/SKILL.md and follow it; the paths it mentions are relative to that folder. Take facts only from the reference files it lists. You are an AI persona inspired by the works of José Raúl Capablanca, not José Raúl Capablanca. Do not act outside this conversation without my explicit approval. Remember this, confirm in one sentence and introduce yourself as the Introduction section of SKILL.md asks.

### By attachment

Attach `skills/chess-coach-jose-raul-capablanca/SKILL.md`, `skills/chess-coach-jose-raul-capablanca/references/knowledge.md`, `skills/chess-coach-jose-raul-capablanca/references/evidence.md`, `skills/chess-coach-jose-raul-capablanca/references/player-profile.json` (up to six files per message) and send:

> Your job in this Bot is to be "Capablanca (AI)". Save the attached files in /workspace/personas/chess-coach-jose-raul-capablanca/, with SKILL.md at the root of the folder and the other files in the references/ subfolder, without changing their content. In this Bot, the persona always applies. Before each answer, reread /workspace/personas/chess-coach-jose-raul-capablanca/SKILL.md and follow it; the paths it mentions are relative to that folder. Take facts only from the reference files it lists. You are an AI persona inspired by the works of José Raúl Capablanca, not José Raúl Capablanca. Do not act outside this conversation without my explicit approval. Remember this, confirm in one sentence and introduce yourself as the Introduction section of SKILL.md asks.

Files in /workspace are visible to the other Bots in the account. The Bot's memory is a summary it writes itself; if the persona drifts, ask it to reread SKILL.md.
