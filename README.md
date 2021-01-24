# Back to the basics

[![PRs welcome](https://img.shields.io/badge/PRs-welcome-green?style=flat-square&logo=github)](https://github.com/maacpiash/ES2017/compare)

Getting a bit tired of frameworks, libraries, `package.json`, and `node_modules`? Me too!

Here, I am trying to develop a whole website with no framework or library: just HTML5, CSS3, and JavaScript (ES2017).

## Why ES2017?

According to [this presentation](https://www.youtube.com/watch?v=cLxNdLK--yI) ([corresponding blog post](https://web.dev/publish-modern-javascript)) at the [Google Chrome Developer Summit 2020](https://goo.gle/cds20-sessions),

> Modern web browsers like Chrome, Edge, Firefox, and Safari make up more than [90% of the browser market](https://www.caniuse.com/usage-table), and different browsers that rely on the same underlying rendering engines make up an additional 5%. This means that 95% of global web traffic comes from browsers that support the most widely used JavaScript language features from the past 10 years, including:
>
>- Classes (ES2015)
>- Arrow functions (ES2015)
>- Generators (ES2015)
>- Block scoping (ES2015)
>- Destructuring (ES2015)
>- Rest and spread parameters (ES2015)
>- Object shorthand (ES2015)
>- Async/await (ES2017)

In a nutshell: if we write (or transpile to) and ship ES2017 code, we can target 95% of the browser market.

## But should we?

Not supporting IE, which now amounts to less than 5% of the global internet traffic, is still a big *no-no* in the web development industry. Opera Mini's extreme mode would also get axed if we exclusively write and ship ES2017. However, my answer to this question is: absolutely yes. According to the aforementioned [presentation](https://www.youtube.com/watch?v=cLxNdLK--yI)/[blog post](https://web.dev/publish-modern-javascript), which I highly suggest checking out, legacy JS requires a significantly larger download, and it is also quite slower — not just because a lot more code is downloaded, but also because it actually **runs slower** in the browser's runtime.

That's right: the same code, when transpiled to an older version of JavaScript, runs drastically slower, compared to the original modern JavaScript code.

## Okay, what else?

I would also like to try out [web components](https://www.webcomponents.org) ([MDN](https://developer.mozilla.org/en-US/docs/Web/Web_Components)). Perhaps, I would give some lightweight CSS/JS libraries a try (using CDN, of course). I have not decided on a build-tool yet.

My affinity for [TypeScript](https://github.com/microsoft/TypeScript) is not brand new information to the people who know me. But, at times, constant type-checking and often-obscure error messages feel exhausting. I will probably give [Hegel](https://github.com/JSMonk/hegel) a try for this project.
