<!-- install/duet.md -->
# Install on Claude Duet

Based on the official documentation checked on 2026-10-25; not yet tested on a real account.

Duet uses the skills and plugins of your Claude account.

1. On claude.ai, open Customize > Plugins > Add > Add marketplace and enter `novantir/kungfukit-publico`. For a private repository, connect GitHub and give the Claude app access. Turn on "Sync automatically".
2. Install the `chess-coach-jose-raul-capablanca` plugin. Alternative: Customize > Skills > Upload with a zip of the `skills/chess-coach-jose-raul-capablanca` folder (the folder must be the top level of the zip).
3. In Duet, send:

> When I ask for "Capablanca (AI)", use the chess-coach-jose-raul-capablanca skill and follow it until I end the mode. Remember this.

To start, ask for "Capablanca (AI)": the persona introduces itself and suggests how to go on.

Duet asks for approval before sending messages, paying, signing or deleting; keep it that way.
