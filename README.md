# Andor's Trail + Duolingo (prototype)

Clean upstream base: [AndorsTrailRelease/andors-trail](https://github.com/AndorsTrailRelease/andors-trail), pinned at `0dfa1f63ea6d944df2c6d34e641000c09d3e917e`.

This repository currently stores an integration patch and a reproducible GitHub Actions build. The build checks out the official source, applies `patches/embedded-duolingo.patch`, then packages an Android debug APK.

Experimental state:
- A **Duo** button opens an embedded Duolingo WebView from combat.
- Real Duolingo sign-in and lesson compatibility have **not** yet been verified.
- Correct answers do **not** yet trigger combat actions.
- There is no accessibility monitoring or modification of the official Duolingo app.

The default debug APK uses the upstream `.dev` application ID suffix, so it is intended for side-by-side testing rather than updating the production installation.
