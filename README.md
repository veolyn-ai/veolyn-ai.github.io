# veolyn-ai.github.io

The organization root of Veolyn AI's GitHub Pages. Nothing lives here: this repository
exists only so that `https://veolyn-ai.github.io` resolves, and its single page forwards
to the research blog.

| | |
|---|---|
| Root | <https://veolyn-ai.github.io/> → redirects to `/blog/` |
| Blog | <https://veolyn-ai.github.io/blog/> — source in [`veolyn-ai/blog`](https://github.com/veolyn-ai/blog) |

The redirect is a `<meta http-equiv="refresh">` plus a `location.replace`, so it works
with JavaScript disabled and carries the query string and hash across. There is no
server-side redirect: GitHub Pages serves static files, so this cannot be a 301.

Keep this repository minimal. Adding a `404.html` here would override the blog's own
not-found page for every path under the domain, so don't.
