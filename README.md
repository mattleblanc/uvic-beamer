## uvic-beamer

A beamer template loosely following the University of Victoria's style guidelines.

## Installation

To install this beamer theme, you can check out the repository into the working directory of your beamer project with:

```
git clone git@github.com:mattleblanc/uvic-beamer.git
```

To use the template, you need to include the header file in your beamer preamble:

```
\input{uvic-beamer/uvic-header.tex}
```

You also need to enclose your first slide in a set of braces, in order to give it the alternative background:

```
% We want this slide to have the other background, with the UVic crest ...
{
\usebackgroundtemplate{
	\includegraphics[width=\paperwidth,height=\paperheight]{uvic-beamer/uvic-title.pdf}
	}
\begin{frame}[plain]
	\titlepage
\end{frame}
}
```

The header has a few options you can play with, feel free to mess around with them to suit your own needs. The default settings get you slides with a 16:9 aspect ratio, and dark blue text.



If you want to build the enclosed example, I'd suggest doing so in a fresh location like this:

```
mkdir myWorkDir && cd myWorkDir/
git clone git@github.com:mattleblanc/uvic-beamer.git
cp -r uvic-beamer/example/* .
make
```

## Tips

There are a few colors defined taken from the UVic brand guidelines, which are available for your general use:

...

## Links

UVic brand guidelines: 
http://www.uvic.ca/communicationsmarketing/assets/docs/UVic-Brand-Guidelines.pdf 

## Disclaimer

This project is totally unofficial. Use at your own discretion.