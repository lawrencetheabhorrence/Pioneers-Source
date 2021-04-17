# Pioneers-Source
Markdown and Latex source files for modules and documents made for the Pi-oneers tutorial service

# How to build
To build PDF files from the Markdown (.md) files you need to install [pandoc](https://pandoc.org/) and a LaTeX distribution with lualatex.
The LaTeX distribution used to build these files is [MiKTeX](https://miktex.org/) which is available for Windows, MacOS, and Linux.

## VSCode Extension
If you are opening the Markdown files in VS Code, you can install the `vscode-pandoc` extension to render files as a PDF. Set the `Pdf Opt String` option to the value
`--from markdown+fancy_lists+startnum --pdf-engine=lualatex`.

## Command line
If you are on the command line, change directory to the folder containing the Markdown file and type:
```
pandoc -o "nameOfYourFile.pdf" --from markdown+fancy_lists+startnum --pdf-engine=lualatext [nameOfYourFile.md]
```
Replace [nameOfYourFile.md] with the filename of the Markdown file you want to render as a PDF, without including the brackets.
