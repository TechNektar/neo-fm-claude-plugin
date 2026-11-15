---
name: make-a-song-for-someone
description: Make an original AI song in an Indian language for a person or occasion, such as a birthday, anniversary or festival, using the user's own neo-fm account. Use when the user asks for a personal song, a song for someone, or a neo-fm song.
---

This skill turns a request for a personal song into a song made in the user's own neo-fm account.

1. Gather four things from the user, asking only for what is missing: what the song is about (in their own words), the language (Hindi, Kannada, Tamil, Telugu, Malayalam, Marathi, Bengali or English), the occasion if any, and the name of the person it is for if the user wants one in the lyrics.
2. Use the neo-fm connector's account status tool first, so you can tell the user how many songs they have left today and this month.
3. Use the neo-fm connector's make-song tool with the user's request. Songs are made in the background, so the first answer is "queued", not a finished song.
4. Use the neo-fm connector's get-song tool to check progress. Show the lyrics when they are available, and say the song is AI-generated.
5. Audio plays only for listeners in India. Outside India, show the lyrics and explain that playback in the assistant is India-only.
6. If the daily or monthly limit is reached, say which limit it is and when it resets. Do not suggest purchases; neo-fm does not sell anything inside the chat.
