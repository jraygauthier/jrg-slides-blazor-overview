Readme
======

A blazor overview reveal-js slide show.

Currently only [available *en français*].

This might come to act as a scaffolding project for subsequent presentation.


Entering the reproducible environment
-------------------------------------

```bash
$ cd /path/to/this/repo
$ nix-shell
# ..
```

The previous steps require [nix].


Building and previewing
-----------------------

## Reveal-js output

```bash
$ cd /path/to/this/repo
$ make revealjs
# ..
$ firefox ./slides-revealjs.fr.html
```

A convenience target is also provided to do the same:

```bash
$ make revealjs-and-preview
# ..
```


Vscode
------

Also, if using *vscode*, make sure to launch it from within the nix environment:

```bash
$ code .
# ..
```

This will allow for the task we setup in `.vscode/tasks.json` to proceed correctly.

 -  `Ctrl + Shift + b`: runs `make revealjs`.


GitHub pages
------------

This slide show is currently hosted on [GitHub Pages].

Here's the link: <https://amotus.github.io/jrg-slides-blazor-overview/>.

The source for the index page is [docs/index.md](./docs/index.md).

GitHub is in charge of rendering `index.md` to a *html* page through
Jekyll.


### Publishing an updated version of the slides

```bash
$ make publish-site
# ..
```

This will make the slides and copy the result to their expected
location under the `./docs/` folder (which GitHub takes as input
for the hosted web site).


License
-------

The markdown document (`*.md`) for the slide show are licensed under
[*Creative Commons Attribution 4.0 International* license](./LICENSE.CC-BY-4).

All accompanying code is licensed under [*Apache 2.0* license](./LICENSE)


Todo
----

A list of various improvements that would enhance this presentation
or this method of doing presentations. See:

[TODO.md](./TODO.md).


[available *en français*]: https://amotus.github.io/jrg-slides-blazor-overview/.
[nix]: https://nixos.org/nix/download.html
[Giphy]:https://giphy.com/
[GitHub Pages]: https://pages.github.com/
