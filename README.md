# ortfo

Central repository for all ortfo-related commands

It registers all ortfo repos as submodules and creates a unified CLI for all of them.

Work in progress.

The role of this is essentially to have a unique binary to do all of what I do in [my portfolio](https://github.com/ewen-lbh/portfolio)'s package.json's scripts.

It should import ortfo* (ortfomk, ortfodb and potentially others) and use them directly.
For others (livescript compiler, stylus compiler, svgo, etc.), when finding a Go library port is not possible,
it should either:

- download it with `npm` (globally?)
- vendor it (seems complicated for node packages which aren't single binaries _at all_)

it should also take care of ortfo*'s external dependencies (ffmpegthumbnailer, pdftoppm, ...)
