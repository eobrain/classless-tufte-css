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
<link rel="stylesheet" href="https://unpkg.com/classless-tufte-css@1.3.0/tufte.min.css"/>
```

(See the [live version][1] for instructions for how to host the CSS and font files yourself.)

Minimal Example
-

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <title>Title Goes Here</title>
    <link rel="stylesheet" href="https://unpkg.com/classless-tufte-css@1.3.0/tufte.min.css" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
</head>

<body>
    <article>
        <h1>Title Goes Here</h1>
        <p>Subtitle goes Here</p>
        <section>
            <h2>Section Header goes here</h2>
            <blockquote>
                <p>Epigraph goes here</p>
                <footer>Attribution goes here</footer>
            </blockquote>
            <p>Main text starts here</p>
            <aside>Margin note goes here</aside>
        </section>
        <section>
            <p>All-caps line goes here</p>
            <ul>
                <li>List item in margin</li>
                <li>List item</li>
            </ul>
            <figure>
                <img src="https://dummyimage.com/2000x200/" />
                <figcaption>Inline figure</figcaption>
            </figure>
            <aside>
                <figure>
                    <img src="https://dummyimage.com/2000x200/" />
                    <figcaption>Margin figure</figcaption>
                </figure>
            </aside>
        </section>
        <section>
            <ul>
                <li>Inline list item</li>
                <li>List item</li>
            </ul>
        </section>
        <figure>
            <img src="https://dummyimage.com/2000x200/" />
            <figcaption>Fullwidth figure</figcaption>
        </figure>
    </article>
</body>

</html>
```
See this [minimal example live][3].



Project Scope and Status
-
Classless Tufte CSS is specifically a CSS-only solution for styling HTML for the web.

That means that JavaScript solutions, although often superior to pure CSS, are out of scope for this project and will not be used. Also out of scope are handling printed versions of web pages and integration with static site generators or other formats. Thankfully, all these useful applications can be well served by separate work that builds on top of Classless Tufte CSS.


Deploying
-
1. Make changes
2. Bump version in *package.json*, examples, and docs to new version with [semver][4] form `X.Y.Z`
3. From shell, `npm install`
4. From shell: `npm publish`
4. Commit changes to git
4. From shell: `git push`
4. From shell: `git tag vX.Y.Z`
4. From shell: `git push --tags`


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
[3]: https://eobrain.github.io/classless-tufte-css/minimal-example.html
[4]: https://semver.org/