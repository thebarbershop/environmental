# environmental

When I'm working in a conda environment, I am too lazy to

<!-- markdownlint-disable no-inline-html -->

1. Open a new terminal with <kbd>⌘ Command</kbd>+<kbd>N</kbd> or <kbd>⌘ Command</kbd>+<kbd>T</kbd>
2. type `conda activate my-conda-environment`.

<!-- markdownlint-enable no-inline-html -->

So I created two shell commands, `window` and `tab`.

Currently supports macOS.

## Install

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

## How to use

```bash
(my-conda-environment) current-directory $ window
```

will open a new terminal window with the same environment at the same directory.

```bash
(my-conda-environment) current-directory $ tab
```

will open a new terminal tab with the same environment at the same directory.