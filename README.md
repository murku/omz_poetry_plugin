# Poetry plugin

This is my personal opinionated plugin for [Oh My ZSH!](https://ohmyz.sh) that adds aliases for my most freqently used [poetry](https://python-poetry.org/)  commands. 

## Installation

* copy the `poetry.plugin.zsh` file to your `$ZSH_CUSTOM/plugins/poetry` folder
```zsh
mkdir $ZSH_CUSTOM/plugins/poetry
cp poetry.plugin.zsh $ZSH_CUSTOM/plugins/poetry
```
* add `poetry` to the plugins array in your zshrc file:
```zsh
plugins=(... poetry)
```
* Reload with `omz reload`
* (Optional) Enable tab completion for poetry (read [poetry doc](https://python-poetry.org/docs/1.8/#zsh))


## Aliases
| Alias     | Command                | Description                                        |
|-----------|------------------------|---------------------------------------------------|
| `poe`     | `poetry`              | Poetry command                                     |
| `poi`     | `poetry install`      | Install dependencies                               |
| `por`     | `poetry run`          | Run command in Poetry environment: `por <command>` |
| `pot`     | `poetry run pytest -s` | Run pytest with output capturing disabled         |
| `poad`    | `poetry add`          | Add a dependency: `poad <package>`                |
| `poadd`   | `poetry add --dev`    | Add a dev dependency: `poadd <package>`           |
| `porm`    | `poetry remove`       | Remove a dependency: `porm <package>`             |
| `mkserve` | `poetry run mkdocs serve` | Run MkDocs development server                 |

[More information about poetry commands](https://python-poetry.org/docs/cli/).
