# environmental

When I'm working in a conda environment, I am too lazy to

<!-- markdownlint-disable no-inline-html -->

1. Open a new terminal with <kbd>⌘ Command</kbd>+<kbd>N</kbd> or <kbd>⌘ Command</kbd>+<kbd>T</kbd> (Or <kbd>Control</kbd>+<kbd>Shift</kbd>+<kbd>N</kbd>/<kbd>Control</kbd>+<kbd>Shift</kbd>+<kbd>T</kbd> or whatever combination of keys you use.)
2. type `conda activate my-conda-environment`.

<!-- markdownlint-enable no-inline-html -->

So I created two shell commands, `window` and `tab`.

Currently supports macOS and Linux (Ubuntu).

## Install

### macOSs

I have developed and tested this tool on __macOS mojave.__

1. Clone the repo.
2. Set permission to run commands.
3. Copy the files so that you can run the commands.

```bash
git clone https://github.com/thebarbershop/environmental.git
sudo chmod +x environmental/mac/*
sudo cp environmental/mac/* /usr/local/bin/
```

Now you may delete the downloaded files, if you don't want to keep them around.

```bash
rm -r environmental/
```

### Linux Users

I have developed and tested this tool on __Ubuntu 18.04 with GNOME 3.28.2.__ To use this tool, you need to install the following two tools.

```bash
sudo apt install xdotool
sudo apt install xclip
sudo apt install wmctrl
```

Then,

1. Clone the repo.
2. Set permission to run commands.
3. Copy the files so that you can run the commands.

```bash
git clone https://github.com/thebarbershop/environmental.git
sudo chmod +x environmental/linux/*
sudo cp environmental/linux/* /usr/local/bin/
```

Now you may delete the downloaded files, if you don't want to keep them around.

```bash
rm -r environmental/
```

## How to use

### window

To open a new terminal window with the same environment at the same directory,

```bash
(my-conda-environment) current-directory $ window
```

### tab

To open a new terminal tab with the same environment at the same directory,

```bash
(my-conda-environment) current-directory $ tab
```