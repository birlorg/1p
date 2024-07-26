# 1password integration with iTerm on macOS.

## Setup:

```sh
brew install choose-gui jq 1password-cli
```

iTerm2/Settings/Keys
click the plus in bottom left and select a key ( I like CMD+/)
action: Run Coprocess

The action should be `1p choose` you probably want to add the full
path to the 1p binary.

You want it to apply to the current session only(i.e. the one you were just typing in.)

The very first time you run it, 1password might prompt you a bunch for access.


## usage: 1p <cmd>

Use one password CLI to choose passwords for terminals
specially designed for iterm2 and macOS by default

 * 1p list  - list all keys in 1P_TAG
 * 1p choose - choose item
 * 1p get <item name>
 * 1p clear  - clear the list cache

## requires:
 * op cli(with biometrics): https://developer.1password.com/docs/cli/
 * jq: https://stedolan.github.io/jq/
 * choose: https://github.com/chipsenkbeil/choose OR https://github.com/sdegutis/choose
    `brew install choose-gui` works

 * iTerm2: https://iterm2.com/

## Troubleshooting:

Ensure ~/.config/1p/ exists and is writeable.
Ensure `op whoami` returns something reasonable.
try running locally outside of the coprocess.
