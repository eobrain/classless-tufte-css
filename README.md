Classless Tufte CSS
=========
This is a modification of the original Tufte CSS to remove reliance on `class`
attributes so it can be applied to purely semantic HTML.

Edward Tufte uses a distinctive style in his handouts: simple, with well-set
typography, extensive sidenotes, and tight integration of graphics and
charts. `tufte-css` brings that style to HTML documents.

This original project was directly inspired by and
based on [Tufte-LaTeX](https://tufte-latex.github.io/tufte-latex/) and the
[R Markdown Tufte Handout](http://rmarkdown.rstudio.com/examples/tufte-handout.pdf).


Getting Started
-
The file *index.html* is a self-describing demonstration document that walks through
the features of Tufte CSS. The live version at
[https://eobrain.github.io/classless-tufte-css/][1]
is the best overview of the project.


To use Tufte CSS, just add the following to your HTML doc's
head block:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/eobrain/classless-tufte-css@v1.0.1/tufte.min.css"/>
```

(See rhw [live version][1] for instructions for how to host the CSS and font files yourself.)


Project Scope and Status
-
Classless Tufte CSS is specifically a CSS-only solution for styling HTML for the web.

That means that JavaScript solutions, although often superior to pure CSS, are out of scope for this project and will not be used. Also out of scope are handling printed versions of web pages and integration with static site generators or other formats. Thankfully, all these useful applications can be well served by separate work that builds on top of Classless Tufte CSS.


Deploying
-
1. Make changes
2. From shell, `npm install`
2. From shell, `npx cleancss -o tufte.min.css tufte.css`
3. Bump version in *package.json*
4. From shell: `npm publish`


Contributing
-

To contribute the original Tufte CSS project see their [Contributing][2] instructions.

Contributions are also welcome to this version in the same way, by opening an
issue, or better yet, a pull request with how you think it should be
fixed.

Contributors
-
 - Dave Liepmann (creator, project maintainer, design)
 - Edward Tufte (editing, direction, design)
 - [Adam Schwartz](https://github.com/adamschwartz) (ET Book font, descender-clearing link underlines)
 - [Clay Harmon](https://github.com/edwardtufte/tufte-css/commits/master?author=clayh53) (media queries, rem units)
 - [Linjie Ding](https://github.com/edwardtufte/tufte-css/commits/master?author=pyrocat101) (italic typeface)
 - [Stephen A Thomas](https://github.com/edwardtufte/tufte-css/commits/master?author=sathomas) (automagically numbered sidenotes)
 - [Ben Newman](https://github.com/edwardtufte/tufte-css/pull/9) (sidenote numbering style)
 - [Kevin Godby](https://github.com/edwardtufte/tufte-css/commits/master?author=godbyk) (booktabs tables)
 - [James Kolce](https://github.com/edwardtufte/tufte-css/commits/master?author=jameskolce) (sidenote fixes)
 - [Chris MacKay](https://github.com/crmackay) (sidenote toggling on small screens)
 - [Paul Rodriguez](https://github.com/edwardtufte/tufte-css/commits/master?author=ruricolist)
   (sidenote style tweaks)
 - [Claudiu-Vlad Ursache](https://github.com/edwardtufte/tufte-css/commits/master?author=ursachec) (HTML5 conformity)
 - [Eamonn O'Brien-Strain](https://github.com/eobrain/classless-tufte-css/commits/master?author=eobrain) (Classless version)


License
-
Released under the MIT license. See [LICENSE](https://github.com/edwardtufte/tufte-css/blob/gh-pages/LICENSE).

[1]: https://eobrain.github.io/classless-tufte-css/
[2]: https://github.com/edwardtufte/tufte-css#contributing
