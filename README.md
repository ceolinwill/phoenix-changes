# Phoenix Changes

Here are the changes I make to every new Phoenix project. I’m documenting them so I don’t have to remember them each time.

## Changes

- Add a [Copilot instructions file](https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file) with commit messages instructions.
- Add LICENSE file.
- Add CODE_OF_CONDUCT.md file.
- Add CONTRIBUTING.md file.
- Sort dependencies alphabetically in `mix.exs`.
- Add [mix_test_watch](https://hexdocs.pm/mix_test_watch).
- Add [TailwindFormatter](https://hexdocs.pm/tailwind_formatter).
- Add [Styler](https://hexdocs.pm/styler).
- Add [Credo](https://hexdocs.pm/credo).
- Add Dependabot configuration.
- Add [sobelow](https://hexdocs.pm/sobelow).
- Add [mix_audit](https://hexdocs.pm/mix_audit).
- Add CI: compile, format, credo, sobelow, unused deps, deps.audit, hex.audit, test.
- Add check for transitive compilation dependencies in CI using [mix xref graph](https://hexdocs.pm/mix/Mix.Tasks.Xref.html#content).
- Add task to update translations: `locale: ["gettext.extract", "gettext.merge priv/gettext"]`.
