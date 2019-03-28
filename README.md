# environmental

When I'm working in a Python virtual environment, I am too lazy to

1. Open a new terminal window/tab with some hotkeys and
2. Type `conda activate my-environment`.

So I created two shell commands, `window` and `tab`.

## Supported environments

### macOS

I have developed and tested this tool on __macOS mojave.__

The tool is available for __conda__ environments.

### Linux

I have developed and tested this tool on __Ubuntu 18.04 with GNOME 3.28.2.__

The tool is available for __conda__ and __virtualenv__ environments.

## Install

### Install on macOS

1. Clone the repo.
2. Set permission to run commands.
3. Copy the files so that you can run the commands.

```bash
git clone https://github.com/thebarbershop/environmental.git
sudo chmod +x environmental/mac/conda/*
sudo cp environmental/mac/conda/* /usr/local/bin/
```

Now you may delete the downloaded files, if you don't want to keep them around.

```bash
rm -r environmental/
```

<!-- markdownlint-disable no-inline-html -->
The script emulates <kbd>⌘ Command</kbd>+<kbd>N</kbd> and <kbd>⌘ Command</kbd>+<kbd>T</kbd> to open a new window/terminal. You have to fix line 8 of each script, if you use a different combination of keys.
<!-- markdownlint-enable no-inline-html -->

### Install on Linux

To use this tool, you need to install the three extra tools, xdotool, xclip, and wmctrl.

```bash
sudo apt install xdotool xclip wmctrl
```

Then,

1. Clone the repo.
2. Set permission to run commands.
3. Copy the files so that you can run the commands.

```bash
git clone https://github.com/thebarbershop/environmental.git
sudo chmod +x environmental/linux/conda/*
sudo cp environmental/linux/conda/* /usr/local/bin/
```

If you use __virtualenv__ instead of __conda__, replace the path accordingly for the last two commands.

Now you may delete the downloaded files, if you don't want to keep them around.

```bash
rm -r environmental/
```

<!-- markdownlint-disable no-inline-html -->
The script emulates <kbd>Control</kbd>+<kbd>Shift</kbd>+<kbd>N</kbd> and <kbd>Control</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd> to open a new window/terminal. You have to fix line 10 of `window` and line 11 of `tab`, if you use a different combination of keys.
<!-- markdownlint-enable no-inline-html -->

## How to use

### window

To open a new terminal window with the same environment at the same directory,

```bash
(my-environment) current-directory $ window
```

### tab

To open a new terminal tab with the same environment at the same directory,

```bash
(my-environment) current-directory $ tab
```

## License

This software is [Unlicenced](https://unlicense.org/). Do whatever you want with it, and I am not liable for any consequences.

## Note

I don't have any plan to import this tool for any other OS or environment manager than the ones I am using. (But I may someday, whenever I feel like it.)

So feel free to fork and modify to fit your own system. I would deeply appreciate if you send me a pull request with your addition.