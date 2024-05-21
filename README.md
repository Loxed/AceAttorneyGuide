Ace Attorney Guide
===

The purpose of this site/guide is to create deeplinks to different guides and resources for the Ace Attorney series, such as the ones on Strategy Wiki. The guides provided by Strategy Wiki are fantastic, however, navigating to specific pages to progress in the games can be a time-consuming process. This site aims to simplify the navigation process by directly linking to the relevant content, making them quickly accessible.

This site was made using mdbook, a tool for creating books with Markdown. The public repository of the site is available [here](https://github.com/Loxed/AceAttorneyGuide) (if anyone wants to fork/contribute).

Note: I mainly made this site for personal fast-access to resources I find useful. However, I hope that others will also find it helpful and contribute to its development if they wish to.

# Prerequisites

To install mdbook, you need to install Rust: [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install)


Run the following command
```rust
cargo install mdbook
```

# How to run

There are several ways to render a book, but one of the easiest methods is to use the serve command, which will build your book and start a local webserver:

```bash
mdbook serve --open
```

The --open option will open your default web browser to view your new book. You can leave the server running even while you edit the content of the book, and mdbook will automatically rebuild the output and automatically refresh your web browser. I personally use ngrok to forward my localhost port to a public http for ui testing on mobile.

# Publishing the book

Execute this command:

```bash
mdbook build
```

This will generate a directory named book which contains the HTML content of your book. You can then place this directory on any web server to host it. Using Railway, pushing the repo auto updates the website.