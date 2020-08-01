# jumpstart
Macbook setup - zero to development

### Initial Macbook setup

Installs

- Google Chrome, iterm2
- zsh ~~with oh-my-zsh~~
- Dropbox, vlc, caffeine, simplenote, the-unarchiver

```
$ ansible-playbook mac.yml
```
### Data analysis setup

Installs
- python
- numpy, pandas, pandas-datareader, matplotlib
- jupyterlab, jupytext
- py_vollib
- statsmodels

```
$ ansible-playbook data-analysis.yml
```
### Manual setup

Currently ansible doesn't have any modules for R packages. We need to manually install a few packages

## Bookdown
```
# Install book down package
install.packages('bookdown')

# For pdf output we need LaTeX distribution. Install TinyTeX (which includes XeLaTeX)
# https://yihui.org/tinytex/
install.packages('tinytex')
tinytex::install_tinytex()
```

## Few more R packages
```
install.packages('rstring')
install.packages('quantmod')
install.packages('tseries')
```
