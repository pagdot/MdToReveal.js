# MdToReveal.js

This repo is about creating [reveal.js](https://revealjs.com/#/) presentations from [Markdown](https://daringfireball.net/projects/markdown/) using [pandoc](https://pandoc.org/).


A markdown file for a sample presentation is [slides.md](slides.md). I've created the reveal.js presentation in [docs/sildes.html](docs/sildes.html). The presentation is also available as [preview via GitHub Pages](https://paul70078.github.io/MdToReveal.js/slides.html).

I plan to extend the sample presentation to be about why to use Markdown to create presentations and hoow to create them with reveal.js and Pandoc's Markdown.

The repository will contain additional samples and more presentation/reveal.js relevant Information. I won't go into detail in the Markdown Syntax because pandoc has already [extensive documentation](https://pandoc.org/MANUAL.html#pandocs-markdown).

## Building the sample presentation

Pandoc needs to be already installed!

The presentation can be build using the following command:

```
pandoc -t revealjs -s --mathjax --slide-level 2 slides.md -o docs/slides.html
```

- `-t revealjs`: Create a reveal.js presentation
- `-s`: Standalone build; Creates HTML file with included reveal.js
- `--mathjax`: Include [MathJax](https://www.mathjax.org/) for math rendering. Because no url is given, mathjax hosted on [mathjax.org](https://www.mathjax.org/) gets used.
- `--slide-level 2`: Create a top-level slide each header 1 and a sub-slide eacher header 2
- `slides.md`: Input file
- `-o docs/slides.html`: Output file

## Contributing

I'd like to get ideas and feedback on how to improve the sample presentation and additional content.

Please use the issues or propose changes in pull requests.

## License

Copyright (C) 2018 Paul Götzinger

Licensed under [GPL 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html)
