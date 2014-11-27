---
layout: post
title: "Markdown example"
date: 2014-06-28 04:43:57 +0200
comments: true
categories: [Test, code]
math: true
---

This is a paragraph, which is text surrounded by whitespace. Paragraphs can be on one
line (or many), and can drone on for hours.

Here is a Markdown link to [Warped](http://warpedvisions.org), and a literal .
Now some SimpleLinks, like one to [google] (automagically links to are-you-
feeling-lucky), a [wiki: test] link to a Wikipedia page, and a link to
[foldoc: CPU]s at foldoc.

<!-- More -->

{% gist be618b71de921ac1a441 dummyExample.js %}

```
$ git clone git@github.com:imathis/octopress.git # fork octopress
```


``` ruby Discover if a number is prime http://www.noulakaz.net/weblog/2007/03/18/a-regular-expression-to-check-for-prime-numbers/ Source Article
class Fixnum
  def prime?
    ('1' * self) !~ /^1?$|^(11+?)\1+$/
  end
end
```

Now some inline markup like _italics_,  **bold**, and `code()`. Note that underscores in
words are ignored in Markdown Extra.


> Blockquotes are like quoted text in email replies
>> And, they can be nested

Below is a bullet list

* Bullet lists are easy too
- Another one
    + Another one

Below is a numbered list

1. A numbered list
2. Which is numbered
    3. With periods and a space with indentation

And now some code:

    // Code is just text indented a bit
    which(is_easy) to_remember();

~~~
// Markdown extra adds un-indented code blocks too

if (this_is_more_code == true && !indented) {
    // tild wrapped code blocks, also not indented
}
~~~

Text with
two trailing spaces
(on the right)
can be used
for things like poems

### Horizontal rules

* * * *
****
--------------------------

<div class="custom-class" markdown="1">
This is a div wrapping some Markdown plus.  Without the DIV attribute, it ignores the
block.
</div>

## Markdown plus tables ##

| Header | Header | Right  |
| ------ | :----: | -----: |
|  Cell  |  Cell  |   $10  |
|  Cell  |  Cell  |   $20  |

* Outer pipes on tables are optional
* Colon used for alignment (right versus left)

## Markdown plus definition lists ##

Bottled water
: $ 1.25
: $ 1.55 (Large)

Milk
Pop
: $ 1.75

* Multiple definitions and terms are possible
* Definitions can include multiple paragraphs too

*[ABBR]: Markdown plus abbreviations (produces an <abbr> tag)

{% pullquote %}
Sed ultricies, metus efficitur maximus suscipit, nulla neque condimentum odio, et dictum leo lectus a ligula. Quisque dignissim sem lorem, quis congue felis fringilla sed. Integer interdum fringilla libero ac mollis. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Praesent[^1] ut imperdiet justo, at hendrerit massa. Morbi ut eros a tortor elementum faucibus. Nunc rhoncus efficitur ultricies. Pellentesque et elit est. Nulla congue gravida velit eget fermentum. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut luctus molestie mi ut interdum. Proin at sodales lectus. Etiam ultrices {" Ut luctus molestie mi ut interdum. Proin at sodales lectus. "} feugiat est, a gravida nunc condimentum sed. Maecenas mauris nulla, varius quis consequat sit amet, faucibus in tortor. Surround your paragraph with the pull quote tags. Then when you come to the text you want to pull,  and that's all there is to it.[^2]
{% endpullquote %}

{% pullquote left %}
Left-aligning pullquotes are good to alternate breaks in the text. They're
{" almost exactly like the default, "} right pullquotes, but a little different.
{% endpullquote %}

{% raw %}
\\[
F(\omega) = \int_{-\infty}^\infty f(t) e^{-i \omega t} \d t.
\\]

\\[
\left( \sum\_{k=1}\^n a\_k b\_k \right)\^2 \leq \left( \sum\_{k=1}\^n a\_k\^2 \right) \left( \sum\_{k=1}\^n b\_k\^2 \right)
\\]
{% endraw %}

This expression \\(\sqrt{3&#215;-1}+(1+x)\^2\\) is an example of an inline equation. 



[^1]: Here's an example of some footnote that should probably explain something.
[^2]: Maecenas mauris nulla, varius quis consequat sit amet, faucibus in tortor. Surround your paragraph with the pull quote tags. Then when you come to the text you want to pull,  and that's all there is to it.