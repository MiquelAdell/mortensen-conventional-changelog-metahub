# **Mortensen's conventional-changelog-metahub**
Check original repo for code. We are just using the readme at the momment.

## Commit types

| Commit Type | Title                    | Description                                                                                                 | Emoji | Release                        | Include in changelog |
|:-----------:|--------------------------|-------------------------------------------------------------------------------------------------------------|:-----:|--------------------------------|:--------------------:|
|   `done`    | done                 | Marks a commit that finishes a feature. This commit should be complete and bugfree                                                                                               |   🎉   | `major`                        |        `true`        |
|   `wip`    | WIP                 | An incomplete feature or bug fix. Check previous commit for what.                                                                                               |   ⚙️   | `minor`                        |        `true`        |
|   `feat`    | Features                 | A new feature                                                                                               |   ✨   | `minor`                        |        `true`        |
|    `fix`    | Bug Fixes                | A bug Fix                                                                                                   |  🐛   | `patch`                        |        `true`        |
|   `docs`    | Documentation            | Documentation only changes                                                                                  |  📚   | `patch` if `scope` is `readme` |        `true`        |
|   `style`   | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      |  💎   | -                              |        `true`        |
| `refactor`  | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                                   |  📦   | -                              |        `true`        |
|   `perf`    | Performance Improvements | A code change that improves performance                                                                     |  🚀   | `patch`                        |        `true`        |
|   `test`    | Tests                    | Adding missing tests or correcting existing tests                                                           |  🚨   | -                              |        `true`        |
|   `build`   | Builds                   | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         |  🛠   | `patch`                        |        `true`        |
|    `ci`     | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |  ⚙️   | -                              |        `true`        |
|   `chore`   | Chores                   | Other changes that don't modify src or test files                                                           |  ♻️   | -                              |        `true`        |
|  `revert`   | Reverts                  | Reverts a previous commit                                                                                   |  🗑   | -                              |        `true`        |

## Commit aliases

Aliases allow to have additional commit types (in a tool like [commitizen](https://github.com/commitizen/cz-cli) for example) that can be formatted to follow [AngularJS Commit Message Conventions](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit).

For example the [commitizen](https://github.com/commitizen/cz-cli) CLI can present the choice `initial` and the final commit message will be 'feat: Initial commit 🎉'

| Commit Type        | Maps to | Title             | Description                     | Emoji  |
|:------------------:| ------- | ----------------- | ------------------------------  |:------:|
| `initial`          | `feat`  | Initial           | Initial commit                  | 🎉     |
| `dependencies`     | `fix`   | Dependencies      | Update dependencies             | ⬆️     |
| `peerDependencies` | `fix`   | Peer dependencies | Update peer dependencies        | ⬆️     |
| `devDependencies`  | `chore` | Dev dependencies  | Update development dependencies | ⬆️     |
| `metadata`         | `fix`   | Metadata          | Update metadata (package.json)  | 📦     |
