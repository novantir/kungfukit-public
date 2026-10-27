<!-- README.md -->
# Capablanca (AI): chess coach from Capablanca's own books

AI persona inspired by the public-domain works of José Raúl Capablanca; unofficial, with no affiliation with or endorsement by heirs or organisations linked to the name, and it is not the person nor speaks for them. Teaches chess to players of any level, in the language they write in, with the methods of Chess Fundamentals (1921), My Chess Career (1920) and a 1922 article: endings first, principles drawn from simple examples, moves explained and games analysed frankly.

Version **1.0.0**, category `chess-coach`, written in English and answering in the user's language. Pilot from assisted curation; quality in a real bot not yet evaluated.

## Install in your bot

| Bot | How |
| --- | --- |
| Grok Bot | [install/grok-bot.md](install/grok-bot.md): send the guide's prompt to the main Grok Bot, which fetches the files through GitHub and creates the persona's Bot; or create the Bot yourself and send the install message. |
| Dots (ChatGPT) | [install/dots.md](install/dots.md): plugin from the repository or install message. |
| Claude Duet | [install/duet.md](install/duet.md): plugin from the repository's marketplace, which also works on claude.ai. |
| Claude Code | `/plugin install chess-coach-jose-raul-capablanca --marketplace novantir/kungfukit-publico` |

In any bot with an instructions field, paste the content of `skills/chess-coach-jose-raul-capablanca/SKILL.md` and attach the files in `skills/chess-coach-jose-raul-capablanca/references/`. On Grok Bot, reading through GitHub and creation through the main Grok Bot were tested on real accounts on 2026-10-26 and 2026-10-27 with other KungfuKit personas (this one has not yet been tested in a bot); Dots and Duet follow the official documentation checked on 2026-10-25, untested.

Once installed, the persona introduces itself and suggests how to start:

- Build a study plan for your level, starting with simple endings.
- Analyse one of your games (PGN) and find the principle that was missing.
- Learn an endgame, middle-game or opening principle from a short example.

## Files

| File | Use |
| --- | --- |
| `skills/chess-coach-jose-raul-capablanca/SKILL.md` | The persona's instructions: AI identification, limits on actions and rules. |
| `skills/chess-coach-jose-raul-capablanca/references/knowledge.md` | Knowledge notes with sources and dates. |
| `skills/chess-coach-jose-raul-capablanca/references/evidence.md` | Rules with evidence, literal excerpts from the works and limitations; the persona quotes from it. |
| `skills/chess-coach-jose-raul-capablanca/references/player-profile.json` | Player profile, empty: fill in only what the player states; null means unknown. |
| `install/` | Install messages for Grok Bot, Dots and Duet. |
| `provenance/persona.json` | Full curated package: rules, evidence excerpts and manifest. |
| `sources.json` | Sources used, with dates and known licence. |
| `package-manifest.json` | Version, targets, validation and hashes. |

## What this persona does and does not do

Does: teaches chess with the methods of Capablanca's works, in the language you write in. It starts from simple endings and draws principles from short examples. It explains why each move is played, helps you analyse your games and builds a study plan for your level.

Does not: it is not Capablanca and does not speak for him. It has no chess engine, so it cannot guarantee exact assessments of positions or long lines; check with an engine when a decision depends on it. It does not teach current opening theory, which has changed a lot since 1921. It promises no rating gains.

## Your profile

The package ships an empty `references/player-profile.json`. The persona asks your level, time control, study time and goal, and uses only what you tell it.

## Sources used

Works by José Raúl Capablanca (1888–1942), in English, quoted in literal excerpts:

- *Chess Fundamentals* (1921)
- *My Chess Career* (1920)
- "Championship Chess: Incidents and Reminiscences" (*The Windsor Magazine*, 1922)

The texts come from Project Gutenberg, Wikisource and archive.org and were consulted in October 2026. The 1934 preface to *Chess Fundamentals* and J. du Mont's preface to *My Chess Career* were left out.

## Public domain

Capablanca died in 1942. His works have been in the public domain in Brazil, the European Union and the United Kingdom since 2013, and in the United States those published up to 1930 are too. The public domain frees the use of the works, but it is not an authorisation from Capablanca or his heirs. That is why the persona carries the name with "(AI)", never speaks as him and only puts the exact words of the works in quotation marks.

## Validation status

22 rules and 17 knowledge notes, drawn from 28 texts: chapters, annotated games and one article. Every rule has literal evidence from at least two different works. Quote locations and the authorship of each text were checked, and the engine checked the public-domain terms.

Two texts by Capablanca were kept out of the curation and have not been read: a 1916 article for development and a 1922 essay for a fidelity test. There has been no evaluation in a real bot and no paid model call.
