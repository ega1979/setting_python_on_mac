# setting_python_on_mac
How to set python 2/3 on some Mac and switch the version which you want to use.

### 1.Install pyenv
```
brew install pyenv
```

### 2. Initialize pyenv: 
```
// Add the following line to ~/.bash_profile or ~/.zshrc
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
```

Enable the setting.
```
source ~/.bash_profile  // In case of bash
source ~/.zshrc         // In case of zsh
```

cf. Check `.bash` or `.zsh` on your mac
```
$ echo $SHELL
/bin/bash // In case of bash
/bin/zsh  // In case of zsh
```


### 3. Install each version of Python
```
pyenv install 3.12.10 // use Python 3.12.10
pyenv install 2.7.18 // e.g. Python 2.7.18
```

### 4. Switch the version of Python
```
pyenv global 3.12.10 // use Python 3.12.10
pyenv global 2.7.18 // use Python 2.7.18
pyenv global system // use default system of python because could not install 2.xx from pyenv
```

Check the version of Python
```
python --version
```

