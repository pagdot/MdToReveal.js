---
title: Presenting with Markdown
subtitle: using pandoc and reveal.js
author: Paul Götzinger
date: 28.11.2018

theme: solarized
revealjs-url: ressources/reveal.js
slideNumber: true
---

# Why Markdown


tyddttymd

## Motivation

Creating presentations fast and easy

## Why create a new one?

![<https://imgs.xkcd.com/comics/standards.png>](https://imgs.xkcd.com/comics/standards.png){width=60%}

## But Powerpoint is simple!

U sure? 

Is it fast to use?

## Modern presentation tools

+ WYSIWYG
  + Powerpoint 
  + LibreOffice Impress 
  + KeyNote
  + Prezi
+ WYSIWYM
  + LaTEX Beamer
  + HTML/JS based presentation tools
    + reveal.js
    + deck.js
    + impress.js

# Markdown for Presentations

## Subslides slide

Part 1

---

Part 2

## Pauses in slides

Part 1

. . .

Part 2

## Fontsizes in text

<small>Small text</small>

~Alternative\ as\ subscript.\ Spaces\ need\ to\ be\ escaped\ with\ `\`~

Normal Text

## Columns

:::::::::::::: {.columns}
::: {.column width="40%"}
Aut recusandae ipsam voluptatem veritatis vel reprehenderit. Ad necessitatibus sint debitis aut quibusdam. Eum quia maxime dolorem.
:::
::: {.column width="60%"}
Et asperiores quis debitis nesciunt. Sed inventore quod odio. At soluta sed sed corrupti et adipisci. Iusto repudiandae sunt accusamus fugit ut sequi. Sequi laboriosam et possimus voluptas molestiae.
:::
::::::::::::::

## Math

There are 2 Possibilities

---

### Inline Math

With Math encapsulated in single `$` you can write inline Math like $a^2 + b^2 = c^2$.

---

### Math blocks

As alternative, you can write math blocks by encapsulating it in `$$`.

$$c = \sqrt{a^2 + b^2}$$

## Source Code

```cpp
/* Generate ASCII Values all numbers */
 
#include <stdio.h>
#include <stdlib.h>
 
int main()
{
    int i=0;
 
    while(i<255) 
    {
        printf("\n \a %d = %c ",i,i);
        i=i+1; 
    }
    getchar();
    return 0;
}
```