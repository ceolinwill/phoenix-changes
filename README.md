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
- Add Prettier to CI.
- Replace `let` with `const` in JavaScript files.
- Increase the `topbar` delay to `1000` to avoid flickixering.
- Replace `heroicons` with `tabler-icons`.
- Remove `finch` from `swoosh` and `application` (use `Req` instead).
- Update favicon and logo.
- Add supported locales to `config/config.exs`.
- Add task to update translations: `locale: ["gettext.extract", "gettext.merge priv/gettext"]`.
- Move `layouts` out of `components`.
- Set `gzip` to `true` in `endpoint.ex`.
- Remove boilerplate from layouts and home controller.
- Adjust `telemetry` formatting to use one line per event.
- Move core components to individual files.
- Add `phx.gen.auth`.
- Remove password authentication.
- Remove "remember me" checkbox.
- Make auth links easier to remember: `/login`, `/signup`, `/logout`.
- Translate auth pages.
- Rename controllers: `MyAppWeb.UserSessionController` -> `MyAppWeb.Controller.UserSession`.
- Rename liveview modules: `MyAppWeb.UserRegistrationLive` -> `MyAppWeb.Live.UserRegistration`.
- Add `@moduledoc` to generated schemas like `User` and `UserToken`.
- Add `gettext` to generated auth files.
- Add `content-security-policy` and fix issues on dev dashboard.
- Use `{0, 0, 0, 0}` for IP address in `config/dev.exs` to test changes in other machines.
- Remove `confirm` page for page confirmation. Instead, create a new route to automatically confirm a user when clicking on the confirmation link.
