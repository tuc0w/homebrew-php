## PHP Support

| PHP Version  | Formula   |
|--------------|-----------|
| PHP 8.2.0    | `php@8.2` |
| PHP 8.2.1    | `php@8.2` |
| PHP 8.2.2    | `php@8.2` |
| PHP 8.2.3    | `php@8.2` |
| PHP 8.2.4    | `php@8.2` |
| PHP 8.2.5    | `php@8.2` |
| PHP 8.2.6    | `php@8.2` |
| PHP 8.2.7    | `php@8.2` |
| PHP 8.2.8    | `php@8.2` |
| PHP 8.2.9    | `php@8.2` |
| PHP 8.2.10   | `php@8.2` |
| PHP 8.2.11   | `php@8.2` |
| PHP 8.2.12   | `php@8.2` |
| PHP 8.2.13   | `php@8.2` |
| PHP 8.2.14   | `php@8.2` |
| PHP 8.2.15   | `php@8.2` |

## Usage
- On macOS, install Xcode Command Line Utilities:
```zsh
xcode-select --install
```

- On Linux, install cURL and Git:
```bash
# Using APT
sudo apt-get install -y curl git
# Using Yum
sudo yum install -y curl git
```
- Install Homebrew:
```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

- If previously installed, update homebrew and the formulae:
```zsh
brew update
```

- If you have packages from old `homebrew/php` tap remove them.

### Add this tap
Fetch the formulae in this tap:
```zsh
brew tap tuc0w/php
```

### Install PHP

> See [PHP Support](#php-support) for available formulae.

- For example, to install `PHP 8.2.12`:
```zsh 
HOMEBREW_PHP_VERSION="8.2.12" brew install tuc0w/php/php@8.2
```

- After installing you have to link it:
```zsh
brew link --overwrite --force tuc0w/php/php@8.2
```

- If you need to have php@8.2 first in your PATH, run:
```zsh
echo 'export PATH="/opt/homebrew/opt/php@8.2/bin:$PATH"' >> ~/.zshrc
echo 'export PATH="/opt/homebrew/opt/php@8.2/sbin:$PATH"' >> ~/.zshrc
```

- Restart the terminal or run `source ~/.zshrc` and test your PHP version:
```zsh
php -v
```
