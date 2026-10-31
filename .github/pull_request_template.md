<!--
Thanks for contributing! The title should follow Conventional Commits, like the commits:
`feat: add stereo depth to opengl games`, `fix: reconnect usb after sleep`.
Types: feat, fix, perf, refactor, docs, test, chore, style.
-->

## What this changes

<!-- What and why, in a few sentences. Screenshots or a short video for anything on screen. -->

Closes #

## Which part

- [ ] Gazeora for Windows (launcher, capture hook, stream server)
- [ ] GazeoraCLI
- [ ] Android app
- [ ] Installer
- [ ] Documentation

## How it was tested

<!-- Delete what doesn't apply, and add what you did. -->

- Built: x64 / x86, with MinGW / MSVC
- Unit tests: `ctest --output-on-failure` passes
- Games: <!-- names, graphics APIs -->
- Stream: <!-- protocol, codec, player or phone -->
- Android: <!-- phone model, Android version -->

## Checklist

- [ ] The code is formatted (`cmake --build build --target format-check`, or the pre-commit hook).
- [ ] New logic has tests, where it can be tested without a GPU or a game.
- [ ] The README and the guides in `docs/` say what changed for users.
- [ ] Commits are small, each one line in Conventional Commits form.
- [ ] I have the right to submit this work, and I've signed the Contributor License Agreement (CLA.md; the bot asks on your first pull request): it's licensed under the GPL version 3 with the terms in NOTICE, and Nithin Aashik may also license it under other terms, including the commercial license.
