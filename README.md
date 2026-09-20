# Windows Media Player – YouTube Edition

A Windows XP-style music player that runs in the browser. Paste a YouTube song or playlist link and it plays with live track info, album art and kaleidoscope visuals.

**Live:** https://dreamtraderafk.github.io/xp-player/

## Features

- Paste a YouTube song or playlist link (auto-plays on paste, or press **Go**)
- Track name, artist and album art update automatically
- Full playlist view, titles fill in as they load
- Visuals: Kaleidoscope, Kaleidoscope Colors, Album Art, Video
- Two skins: Media Player 8 and Media Player 9
- Play, pause, stop, previous, next, seek, volume, mute, shuffle, repeat
- Working menus, Media Library (recent links saved on your device)
- Works on phone and desktop
- Keyboard: `Space` play/pause, `←` `→` seek, `↑` `↓` volume, `N` next, `P` previous

## Usage

1. Open the live link
2. Paste a YouTube link into **Address**
3. Press **Go**
4. Change visuals and skin from the **View** menu

### Share a link that loads a song

Add `?u=` and a YouTube link to the URL:

```
https://dreamtraderafk.github.io/xp-player/?u=https://youtu.be/VIDEO_ID
```

## Supported links

- `youtube.com/watch?v=…`
- `youtu.be/…`
- `music.youtube.com/…`
- `youtube.com/playlist?list=…`
- Plain video or playlist IDs

## Run it yourself

It is a single file, `index.html`. No build step, no dependencies.

- **GitHub Pages:** upload `index.html`, then **Settings → Pages → Deploy from a branch → main / root**
- **Locally:** `python -m http.server`, then open `http://localhost:8000`

> Opening the file directly (`file://`) won't work. YouTube blocks embeds from local files, so it must be served over http or https.

## Limitations

- The kaleidoscope pulses to a fixed beat, not the actual audio. YouTube does not expose audio data to pages.
- YouTube Mix (`RD…`) playlists can't be embedded.
- Some videos block playback outside YouTube and will be skipped.
- If nothing starts on a phone, open **View → Video** and tap the video once.

## Disclaimer

Fan-made tribute to the Windows XP-era player. Not affiliated with Microsoft or Google. Playback is provided by the official YouTube embedded player.
