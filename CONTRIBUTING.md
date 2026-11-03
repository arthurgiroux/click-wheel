# Contributing

- One small change per pull request.
- Before you push, run the three commands in the README.
- Do not commit device backups. Use `fixtures/private/`, which Git ignores.
- Keep layers separate: a crate calls only the crate directly below it.
- Parsers must never panic on bad input.
- Use only GPL-compatible dependencies. `cargo deny check` must pass.
