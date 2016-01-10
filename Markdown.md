# Markdown Basics

## Paragraphs
Paragraphs are really easy.  It's just text followed by more than one blank lines, like a real paragraph.

This is a new one.

## Headings
The number of # used indicates the level of heading.  # is a top level heading.  ## is a second level heading and so on.  They don't work without the space.  You just get #hashtags.

## Blockquotes
Use a > to start a blockquote.
> Like this.
>
> Here's a continuation

## Styling text
You can do **bold** or *italic* with stars.  One star for italics.  Two stars for bold.
Underscore also works.  __bold__ and _italic_.  _**Combined**_ for both!

## Lists
Unordered lists use either a * or -:

* Item 1
* Item 2
* Item 3
- Item 4

Ordered lists use numbers.  Make sure you add a blank line before the list starts.  The numbers used don't actually matter.  The next lines all start with `1.`.

1. Item 1
1. Item 2
1. Item 3
1. Item 4

Nested lists use two spaces.

1. Item 1
  2.  Sub item 1
  2.  Sub item 2
1. Item 2
  * Sub item 1
  * Sub item 2

## Code formatting
Use backticks for monospace formatting.

`Where the hell is the backtick key?`

You can do full paragraphs too by starting and ending with a line of triple backticks:
```
Haikus are easy
But sometimes they don't make sense.
Refridgerator.
```

## Links
The text of the link goes in square brackets, and the target goes in parentheses.  For example, most of [this](https://help.github.com/articles/markdown-basics/) comes from github.com.

# Github additions (that work in atom)

## Strikethrough
~~strikethrough~~ is done by surrounding the striken text with two tildes.

## URL Autolinking
Full urls autolink, according to https://help.github.com/articles/github-flavored-markdown/.

## Syntax highlighting for languages!
Syntax highlighting for languages!  Three backticks to start followed by the language you want to highlight.

Use c++ for c++
```c++
#include <stdio>

void main()
{
  printf("Cool!");
}
```

Use cs for csharp
```cs
using System;

namespace Foo
{
  public static class Program
  {
    public static void Main(string[] args)
    {
      Console.WriteLine("Cool!");
    }
  }
}
```

## Tables
Hyphens for the first row, pipes to separate columns.  You need at least 3 hyphens per column in the hyphen row.  Formatting also works.

```
First Header | Second Header
---|---
_Cell 1_ | **Cell 2**
Cell 3 | ~~Cell 4~~
```

results in

First Header | Second Header
---|---
_Cell 1_ | **Cell 2**
Cell 3 | ~~Cell 4~~

Colons in the hyphen row changes alignment.  Left for left, both for center, right for right:

```
Left | Center | Right
:----|:------:|-----:
1 | 2 | 3
4 | 5 | 6
```

Left | Center | Right
:----|:------:|-----:
1 | 2 | 3
4 | 5 | 6

## Task Lists
Unordered list identifier followed by square brackets with either a space (for not done) or an x (for done):

- [ ] Not done
- [x] Done!
- [x] _Markdown_ works in here too
  - [ ] **nesting** works too

## Images
Hyperlink with a leading !

`![alt text](media/Profile.jpg "Tool tip text")`:

![alt text](media/Profile.jpg "Tool tip text")

References also work

```
![alt text][profile]

[profile]: media/Profile.jpg "Reference tool tip text"
```

![alt text][profile]

[profile]: media/Profile.jpg "Reference tool tip text"
