# neo-fm

Original AI songs and radio in Indian languages, from your own neo-fm account, inside Claude.

neo-fm makes songs in Hindi, Kannada, Tamil, Telugu, Malayalam, Marathi, Bengali and English for people and occasions: birthdays, anniversaries, festivals, friendships. This plugin connects Claude to your neo-fm account and adds a skill, "make a song for someone", that gathers what is needed and asks neo-fm to make the song.

Publisher: TechNektar. Website: https://www.neo-fm.com

## What it adds

- **A connector** to the neo-fm server at `https://www.neo-fm.com/api/assistant/mcp`. You sign in with your neo-fm account through OAuth the first time you connect. Claude can then check your account status (songs left), start a song, check its progress and lyrics, and list your own recent songs.
- **A skill**, `make-a-song-for-someone`, that guides Claude through making a personal song.

## What you should know

- **Every song is AI-generated.** neo-fm labels it as AI-generated music, and Claude is told to say so.
- **Playback in Claude is for listeners in India only.** The check is made on the device that fetches the audio. Outside India you still get the lyrics, and a link to the song on neo-fm.com.
- **There is a free tier, with limits.** Your plan's monthly allowance applies, and assistants have an extra cap of 2 songs a day per person. The exact numbers for your account come from `account status`; they are not fixed in this plugin.
- **No purchases in chat.** Nothing is sold, no upgrade is offered and there is no checkout inside Claude. Account and plan questions go to your neo-fm account page at https://www.neo-fm.com/account.
- **Invite-only sign-up.** You need an existing neo-fm account to connect.

## Data

The plugin sends the text of the song request you give Claude (for example the occasion, mood, language and an optional recipient name) to neo-fm at www.neo-fm.com, together with your account sign-in. It does not read your Claude memory, chat history or files, and it contacts no other service. The plugin itself stores nothing. neo-fm keeps your songs and account details under its privacy policy.

## Privacy, terms and contact

- Privacy policy: https://www.neo-fm.com/privacy
- Terms: https://www.neo-fm.com/terms
- Support: support@technektar.com
- Grievance and support: support@technektar.com

## Install

- **claude.ai or Claude desktop**: Customize > Plugins, then add this plugin, then open its Connectors tab and connect neo-fm.
- **Claude Code**: `claude plugin marketplace add TechNektar/neo-fm-claude-plugin` then `claude plugin install neo-fm@technektar`.
- **Connector only**: add `https://www.neo-fm.com/api/assistant/mcp` as a custom connector.

When adding neo-fm in Claude, the dialog may say "No sign-in". Choose "Sign in now", or connect when the first account tool asks, to link your neo-fm account. The label appears because neo-fm's link tools work without an account; linking still works.

## License

Copyright (c) 2026 TechNektar. All rights reserved. neo-fm is proprietary; this repository contains only the plugin wrapper (manifest, connector config, skill, icon) and no neo-fm code. Do not copy, redistribute or fork. See LICENSE. Use of the neo-fm service is governed by https://www.neo-fm.com/terms.
