# 1password integration with iTerm on macOS.

install choose-gui
        echo "usage: 1p <cmd>"
        echo '  Use one password CLI to choose passwords for terminals'
        echo ' specially designed for iterm2 and macOS by default'
        echo
        echo '  1p list'
        echo '          list all keys in 1P_TAG'
        echo '  1p choose'
        echo '          getpw ITEM from 1P_TAG using FZF or other chooser.'
        echo '          adds a special item named 'clear' which will clear'
        echo '           the cache and let you choose again.'
        echo '  1p get <item name>'
        echo '          getpw ITEM from 1P_TAG'
        echo '  1p clear'
        echo '          clear the list cache'
        echo
        echo 'requires:'
        echo '  op cli(with biometrics): https://developer.1password.com/docs/cli/'
        echo '  jq: https://stedolan.github.io/jq/'
        echo '  on MacOS:'
        echo '          choose: https://github.com/sdegutis/choose'
        echo '  otherwise:'
        echo '          fzf: https://github.com/junegunn/fzf'
