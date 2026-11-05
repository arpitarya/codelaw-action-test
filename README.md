# codelaw-action-test

The proof of [codelaw](https://github.com/arpitarya/codelaw)'s GitHub Action
(**codelaw check**): `.github/workflows/codelaw.yml` runs
`uses: arpitarya/codelaw@v0` on a fixture with one known finding — the
`debugger` in `src/app.js`, an error by the local rule
`.codelaw/rules/fixture/no-debugger.md`. Each run annotates it, uploads SARIF
to Security → Code scanning, and asserts exit code 1.

The finding is deliberate; do not fix it.
