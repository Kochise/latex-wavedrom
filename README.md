# latex-wavedrom
LaTeX package to interface with wavedrom (npm)

Source : https://github.com/Kochise/latex-wavedrom

## installation

Get 'nvm' for Windows : https://github.com/coreybutler/nvm-windows/releases<br>
Uncompress/install it where you need.<br>

```batch
\>cd nvm
\nvm>nvm install 12.17.0
\nvm>nvm use 12.17.0
\nvm>node -v
v12.17.0
\nvm>npm install -g wavedrom-cli

xcopy /c /h /e /r /q /y latex-wavedrom <miktex>\texmfs\install\tex\latex\wavedrom
start "" "<miktex>\miktex-portable.cmd"
```

Refresh the filename database.<br>
Update the package database.<br>
You should be ready to go.<br>

Alternatively, you can use https://github.com/Kochise/win_portable

## usage

See https://github.com/wavedrom/cli<br>

In your preamble :

```latex
\def\imagepath{./images}
\graphicspath{{\imagepath/}}
\usepackage[imagepath=\imagepath]{wavedrom}
```

In your document :

```latex
% https://wavedrom.com/editor.html
%\begin{wavedrom}[width]{caption}{refname}
\begin{wavedrom}[8cm]{wavedrom caption example}{wavedromexample}
{signal: [
  {name: 'clk', wave: 'p.....|...'},
  {name: 'dat', wave: 'x.345x|=.x', data: ['head', 'body', 'tail', 'data']},
  {name: 'req', wave: '0.1..0|1.0'},
  {},
  {name: 'toto', wave: '1.....|01.'}
]}
\end{wavedrom}
```

## options

Not much available.

## limitations

Your imagination.

## greetings

Based on https://github.com/dakusui/latex-ditaa<br>
Also interested into https://github.com/sile-typesetter/sile<br>
