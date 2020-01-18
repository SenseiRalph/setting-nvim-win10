# Setup

This is for getting a Neovim GUI working on Windows 10 with your init.vim and solarized theme. Tested on a PC and laptop. Your mileage may vary.

**Step 1**: Install Chocolatey (https://chocolatey.org/install).

**Step 2**: Install Neovim from cmd as admin (https://github.com/neovim/neovim/wiki/Installing-Neovim).

**Step 3**: Install a Neovim GUI. I chose Fvim (https://github.com/yatli/fvim) among the many available. Recommended. (Note: first startup of this GUI might take a minute.)

**Step 4**: Put your `init.vim` in C:\Users\yourname\AppData\Local\nvim. This is where Neovim looks for the config.

**Step 5**: Now you need to set a `%HOME%` environment variable. Go in your environment variables, and under the variables for your account, add `HOME` with the path of your choice.

**Step 6**: Go in your `HOME` folder and add a directory named `.vim` (use cmd if Windows does not let you do it in the file explorer). In it, create a folder `bundle`.

**Step 7**: Download Vundle, the vim plug-in manager (https://github.com/VundleVim/Vundle.vim). Just download the zip and paste the whole extracted folder `Vundle.vim-master` in the `bundle` folder you just created. Rename it to `Vundle.vim`.

**Step 8**: Install the theme. Download the flattened theme (https://github.com/romainl/flattened) and paste `flattened-master` in the `bundle` folder. Rename the folder to `flattened`. (Note: I tried using the original solarized by Ethan Schoonover, but the colours always got back to the default ones. Also tried solarized8 to no avail.)

**Step 9**: Setup your init.vim. Just follow the .vimrc instructions on the Vundle page. Then add `Plugin 'flattened'` to the Vundle part of your config. Finally, add `colorscheme flattened_dark` to your init.vim.

You're done! Open your Neovim GUI and feast your eyes. If you encountered problems, you shouldn't be surprised. Mess around and try to find the culprit!
