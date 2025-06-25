# Config Files

## zsh

`~/.zprofile`

```zsh
# set homebrew paths
eval "$(/opt/homebrew/bin/brew shellenv)"

# set uv (and other rust tools) path
source $HOME/.cargo/env

# set local path
export PATH="$HOME/.local/bin:$PATH:/Library/Developer/CommandLineTools/usr/bin"
```

`~/.zshrc`

```zsh
# modern alternates
alias ls='eza'
alias la='eza -a'
alias ll='eza -alh --git'
alias vi='hx'

# shell options
setopt INTERACTIVE_COMMENTS
setopt HIST_IGNORE_ALL_DUPS
bindkey '^[[A' up-line-or-search
bindkey '^[[B' down-line-or-search

# shell autocomplete
fpath+=$HOME/.zfunc
autoload -Uz compinit
compinit

# uv completion
eval "$(uv --generate-shell-completion zsh)"
eval "$(uvx --generate-shell-completion zsh)"

# starship completion
eval "$(starship init zsh)"
```

## ghostty

`~/.config/ghostty/config`

```zsh
theme = MaterialDarker
macos-titlebar-style = tabs
mouse-hide-while-typing = true
```

## helix

`~/.config/helix/config.toml`

```toml
theme = "material_darker"

[keys.normal]
Z = { Z = ":wq" }
D = "kill_to_line_end"
"#" = "toggle_comments"
```

`~/.config/helix/languages.toml`

```toml
[[language]]
name = "python"
language-servers = ["basedpyright", "ruff"]
auto-format = true
formatter = { command = "ruff", args = ["format", "-" ] }
file-types = ["py"]
roots = ["pyproject.toml", "uv.lock"]

[[language]]
name = "rust"
language-servers = ["rust-analyzer"]
auto-format = true
formatter = { command = "rustfmt" }
file-types = ["rs"]
roots = ["Cargo.toml", "Cargo.lock"]

[[language]]
name = "cpp"
language-servers = ["clangd"]
auto-format = false
formatter = { command = "clang-format" }
file-types = ["cpp","hpp","ino"]

[[language]]
name = "c"
language-servers = ["clangd"]
auto-format = false
formatter = { command = "clang-format" }
file-types = ["c","h"]

[[language]]
name = "markdown"
auto-format = true
formatter = { command = "mdformat", args = ["-"] }
file-types = ["md"]
text-width = 100
soft-wrap = { enable = true, wrap-at-text-width = true }
```
