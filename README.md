# Power Search and Autocomplete


# Why PCHAA?
- FOSS
- Not Electron based
- Works with your existing terminal & shell
- Customize text search algorithms as per your need

# Demo

(old gif, please use `pchaa` instead of `python main.py`)
![pchaa](https://user-images.githubusercontent.com/6279035/177213296-1e8af323-fd62-4f1b-a8c5-89e2e99d6701.gif)

# Project Goals

The goal of the project is to create a beautiful experience for Terminals users. All of the alternative versions for such projects were ElectronJS based, I needed something minimal with easy to update custom search algorithms

**Install**
```
# Install xdotool, for arch linux its
sudo pacman -S xdotool

pip install python-libxdo prompt_toolkit 
pip install pchaa
```

**Run**
```
pchaa
```

## Next steps:

Clean and filter the bash history and integrate Naive Bayes algorithm for next command prediction

--- 

**Similar projects**

- https://fig.io/
- https://www.warp.dev/
- https://www.hyper.is
- https://github.com/mflorence99/el-term


# FAQs
## My auto complete window is empty
pchaa uses ~/.bash_history to get previously used bash history. Make sure your terminal has some history to be displayed.

## Does pchaa work in tty?
pchaa uses xclip which needs X running. pchaa won't work in wayland/ tty as of now.

## Wayland and MacOS fix
- wtype, wl-clipboard, wclip, ydotool
- pbcopy and pbpaste, If anyone wan'ts this to port to MacOs feel free to file an issue, I need a user to test.
