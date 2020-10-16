# Thanks to the original creator of the imp-template2 project
https://glitch.com/edit/#!/imp-template2
# What I, [MG]Octo#9071 have changed
- FPS Improvements
- Moved Token Imput
- Added a functional server selector
- Fixed outdated connection stuff for things like Heroku
- Few Little Things
- More like original arras.io changelog
# How to add your server(s)
- Go to line 3339 in bundle.js
- You'll see there are multiple things that look like this:
- `          {
- `           visible: 0,
- `           id: "1",
- ``           type: "game",
- ``           code: "glitch-worldwide-f",
- ``           at: p.glitch('your-server'),
- ``           prefer: !0,
- ``          // featured: 1, // For Featured Status.
- ``         },`