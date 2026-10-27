<!-- install/dots.md -->
# Install on Dots (ChatGPT)

Based on the official documentation checked on 2026-10-25; not yet tested on a real account.

## As a plugin (preferred)

The repository has the plugin in Codex format (`.codex-plugin/plugin.json`) and the skill in `skills/chess-coach-jose-raul-capablanca/`. In the ChatGPT desktop app, add the repository's marketplace (`codex plugin marketplace add novantir/kungfukit-publico`), restart the app and install "Capablanca (AI): chess coach from Capablanca's own books" from the plugin directory. The documentation does not say whether Dots uses skills from plugins; check by asking it to list the available skills.

## Through the chat (alternative)

Send your Dot the message below, then paste the content of `skills/chess-coach-jose-raul-capablanca/SKILL.md`, `skills/chess-coach-jose-raul-capablanca/references/knowledge.md`, `skills/chess-coach-jose-raul-capablanca/references/evidence.md`, `skills/chess-coach-jose-raul-capablanca/references/player-profile.json`.

> When I ask for "Capablanca (AI)", use the instructions and references I am about to send until I end the mode. Keep them in your notes without summarising the rules. You are an AI persona inspired by the works of José Raúl Capablanca, not José Raúl Capablanca. Do not act outside the conversation without my approval. Confirm in one sentence.

## Suggested custom rules

In Settings > Personalization > Permissions > Custom rules: "ask first" for sending messages and publishing; "hand over to me" for purchases and deletions.

To start, ask for "Capablanca (AI)": the persona introduces itself and suggests how to go on.
