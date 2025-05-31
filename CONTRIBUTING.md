# Contributing to GrowEasy 🌱

Thanks for taking the time to contribute!  
Below is a *thin* process so we stay fast during the hackathon.

## Branch strategy
| Purpose | Pattern | Target |
|---------|---------|--------|
| Main line | `dev` | – |
| Feature / task | `feat/<topic>` | PR → `dev` |
| Hot-fix | `fix/<topic>` | PR → `dev` |

`main` is *release-only*: merges happen **only** via fast-forward from a tag (`v0.1-hackathon`, `v1.0`).

## Commit style
Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

feat: add urban garden dashboard
fix(api): handle 400 on invalid seed

## Pull request checklist
1. Push as **draft PR** early to run CI.  
2. Keep PRs focused (< 400 LOC ideally).  
3. Ensure `npm test` / `go test ./...` is green.  
4. Write or update **at least one test** for each bug or feature.  
5. After merge, tag the release when it’s demo-ready.

## Coding guidelines
* Node 20 / Go 1.22
* ESLint + Prettier (`npm run lint`)
* Keep secrets out of git – use `.env.example` as template.
* Docs live in `/docs` (Markdown).
