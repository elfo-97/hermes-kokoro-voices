# hermes-kokoro-voices

The voice samples page for [hermes-kokoro-tts](https://github.com/elfo-97/hermes-kokoro-tts): 54
voices in 9 languages from the Kokoro-82M model, each one with an HTML5 player and the command that
selects it.

Live at https://hermes-kokoro-voices.vercel.app

Static, and nothing else: `index.html` plus `audio/` is the whole page. No build step, no framework,
no external requests, no JavaScript beyond the copy buttons. The clips are the same MP3s that ship
in the plugin repo under `samples/`.

Every voice is an anchor, so `https://hermes-kokoro-voices.vercel.app/#pf_dora` links straight at
one.

The page is generated from the plugin's own voice catalog by `tools/build_site.py` in the plugin
repo. To update it, run that script there and copy `docs/index.html` and `docs/audio/` over here.

MIT, see [LICENSE](LICENSE).
