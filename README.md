# How to Integrate Git Status Indicators into the Bash Prompt

<h4 align="center">How to add git status information inside the bash prompt</h4>
<h5 align="center"><a href="https://jamyvetter.net/posts/how-to-integrate-git-status-indicators-into-the-bash-prompt/">Full article here</a></h5>

<p align="center">
  <a href="https://github.com/jamyvetter/bash_gitprompt/issues">
    <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat">
  </a>
  <a href="https://jamyvetter.net/posts/how-to-integrate-git-status-indicators-into-the-bash-prompt/">
    <img src="https://img.shields.io/badge/%20-jamyvetter.net-2C3E50?style=flat&labelColor=7F6754&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAAXNSR0IB2cksfwAAAAlwSFlzAAALEwAACxMBAJqcGAAAAYNQTFRFAAAAAgkbAQ4oAg4qFg4xBQwmEggmAQwkAA8qARAsAg8rKg48qQxypwtulQtoAAwhABArABAsAQ8sAg8sEw4y1wyF/AyV8w2SAA8qWg1Q/gyW/AyVAA0lABAtBQ0pwwx8/gyV+A2TAA8rABAtDA8vXw1T0wyE/AyUAA4nARItBi9NCTteCTpdBypHCg4tdgxc+QyU+QyUAwoaABAsARQxDV6IFYa4E3elDluGC053DE94D16JFHimF4S1E1J9ShBL8AyQAA8oCDteEGiTBjRVABItAhEtDTRZUzmKvg9/+gyUDFB1C0VpVFlnWVxrDRs1AA8sGiU8aWt3Nz5RAw8rBA4qcw1b/AyUF4GuEyA5c3V+XWBtAREsBxUwb3B7Z2l1CxcxBA8rBg4q4g2KHanlAhk2HQ018QyRHbb1FH2uABEuwgx99g2RHbX3EnSjABIvCw4tuQ58+g6dHLP4Em6aARMvDQ8vrw557hCZJsr5DlNyABEtAQ8rAQ8sCA8tgxBp/BGoSgeKTgAAAIF0Uk5TAAF05ttaABvH/////7AOFOX//////88JpP//cDP7///yFsP/////jVD/////////+yUB1v///////////////6Vi//////////0w0v/9/P///v7+////qPf//f3//v38////5Mf//6M2+P/wIDrn///pLBjC//+8HAWK/v/++m8Ec4VCOAAAALxJREFUeJxjZAABRjD4BWaCCHaIAOMnqAA/I+MPTrDIS4iAxE8Ghh9c34HiT8ECMoxfQPQPEaCS+yABJSB+x8AoxMj4hfcmUEDjN8M7CZABd1SBxHlGI0YUcIDREUSdAbvABCzkzXiUwYaR8ZA9TE3EaYZ3HlD2F14gkcK4D2gH0CEMjF4MvKyMjBmMjDvhArdsGRkZchkZF0EFZBgZ+4COKmZknAO04ztjDiNjB9gvlYyM0xiyQaY2MDAAAGiFKeiOfi4zAAAAAElFTkSuQmCC" alt="Jamy's badge">
  </a>
</p>



<p align="center">
  <a href="#features">Features</a> •
  <a href="#installation-instructions">Installation</a> •
  <a href="#-notes">Notes</a>
</p>

---

# Features

- Displays current Git branch in the bash prompt.
- Shows Git status indicators for uncommitted changes (`⚡`), ahead (`↑`), behind (`↓`), or diverged (`↕`) states relative to remote.
- Automatically updates prompt with color highlighting.
- Sets the terminal/tab title dynamically with username, hostname, and current directory.
- Shows a red ✘ symbol when the last command failed.
- Compatible with xterm, rxvt, and vte-based terminals (including WSL2 + Windows Terminal).

# Installation Instructions

1. Clone or download this repository:
   ```bash
   git clone https://github.com/jamyvetter/bash_gitprompt.git
   ```

2. Source the `bash_gitprompt` script at the end of your `~/.bashrc`:
   ```bash
   source /path/to/bash_gitprompt/.bash_gitprompt
   ```

3. Reload your shell configuration:
   ```bash
   source ~/.bashrc
   ```

4. Start a new terminal or run commands to see your enhanced prompt with Git info.

# 📋 Notes

- Requires `git` to be installed and available in your `$PATH`.
- Relies on the presence of a Git repository to show branch and status info.
- Tested on WSL2 (ubuntu 22.04).
- Colors and symbols can be customized by editing the `.bash_gitprompt` file.
- Terminal/tab title updating works in most xterm-compatible terminals.


If you encounter any issues or have feature requests, please open an issue.
