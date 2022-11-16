# Setting up for dev on a Mac

## A tool for installing software - brew

Brew will be your goto tool for installing software. Learn about and get brew from: https://brew.sh/

Install with the command...
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

At the end of the install run the commands...
```
echo '# Set PATH, MANPATH, etc., for Homebrew.' >> /Users/sbarlster/.zprofile
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/sbarlster/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## JavaScript

You cant get away from the goto language of the web and why would you want to. And once you have JS you
will then have access to TypeScript too. Node is most likely the runtime you will use for JS.

First a tool to manage versions of node - nvm...
```
brew install nvm
```

