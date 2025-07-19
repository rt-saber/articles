# Phrack Articles for <https://phrack.org>

This repository contains PHRACK articles as TXT and as Markdown. Changes to these files will update the articles at <https://www.phrack.org>.

Anyone, but mostly authors, are encouraged to send PullRequests to fix or update an article.

Examples PHRACK articles using MarkDown:
* <https://staging.phrack.org/issues/71/6_md>
* <https://staging.phrack.org/issues/71/7_md>
* <https://staging.phrack.org/issues/71/8_md>

How to add Markdown-beauty to an article:

1. Change to the directory containing the ascii articles: `cd issues/71/`
1. Example: `cp 9.txt 9.md`
2. Add a `<PRE>` a the beginning (*See [helloworld.md](/examples/)*).
1. Start `docker run --rm -p8080:80 -v"$(pwd):/src" -it phrackzine/mdbuilder`
1. View the rendered article at [http://localhost:8080](http://localhost:8080).
1. Add Markdown tags, especially syntax highlights, to make the article look more pretty.
1. Create a PR at [phrackzine/articles](https://github.com/phrackzine/articles) for the Markdown article.

---

### Markdown Tips

Open your favorite editor and add Markdown tags to your `9.md`.
* You may need to convert some `<` and `&` to `&lt;` and `&amp;`.
* Keep most of the article inside a `<PRE>`-block. Use `</PRE>` before using any markdown syntax.
* Don't forget to add `<PRE>` after you are done using Markdown syntax.
* All available Markdowns: [https://daringfireball.net/projects/markdown/syntax](https://daringfireball.net/projects/markdown/syntax)
* All available Syntax Highlights [https://pygments.org/languages/](https://pygments.org/languages/).

