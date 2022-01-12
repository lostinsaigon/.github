### Hi there 👋

[![tatsy's github stats](https://github-readme-stats.vercel.app/api?username=tatsy)](https://github.com/anuraghazra/github-readme-stats)

<!--
**tatsy/tatsy** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

# saigonese.io
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/hzlzh/Mou-Theme?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Both `Themes` and `CSS` for [MacDown](http://macdown.uranusjr.com/) & [Mou.app] \(A nice MarkDown editor on Mac OS\)  
_Repo Path:_

    --- 
     |---- CSS/             CSS Style files  
     |---- Themes/          Mou's `Code Mode` Theme  
     
## Includes

### CSS: GitHub ReadMe Style v1.1
markdown-it-responsive
===

[![Build Status](https://travis-ci.org/tatsy/markdown-it-responsive.svg)](https://travis-ci.org/tatsy/markdown-it-responsive)
[![NPM version](https://img.shields.io/npm/v/markdown-it-responsive.svg?style=flat)](https://www.npmjs.org/package/markdown-it-responsive)
[![Coverage Status](https://coveralls.io/repos/tatsy/markdown-it-responsive/badge.svg)](https://coveralls.io/r/tatsy/markdown-it-responsive)

> A markdown-it plugin for responsive images. This plugin overloads original image renderer of markdown-it.

## Usage

### Enable plugin

```js
var md = require('markdown-it')({
  html: true,
  linkify: true,
  typography: true
}).use(require('markdown-it-responsive'), options);  // <-- this use(package_name) is required
```

### How to specify options?

The notation to specify responsive sizes is as follows.

```js
var option = { responsive: {
    'srcset': {
      'header-*': [ {
        width: 320,
        rename: {
          suffix: '-small'
        }
      }, {
        width: 640,
        rename: {
          suffix: '-medium'
        }
      } ]
    },
    'sizes': {
      'header-*': '(min-width: 36em) 33.3vw, 100vw'
    }
  }
};
```

### Example

With the options above, a markdown

```md
![test](header-test.png)
```

is rendered as

```html
<p><img src="header-test.png" srcset="header-test-small.png 320w, header-test-medium.png 640w" sizes="(min-width: 36em) 33.3vw, 100vw" alt="test"></p>
```




[GitHub-ReadMe.css] is a CSS Style for Mou's `Code Mode`, it shows exactly what `ReadMe.md` will look on GitHub page, enjoy~

Screenshot:  
![GitHub-ReadMe-Preview.png](https://github.com/hzlzh/Mou-Theme/raw/master/CSS/GitHub-ReadMe-Preview.png)

### Theme: Sublime v1.1

[Sublime.txt] & [Sublime+.txt] are CSS Styles for Mou's `Live Preview Mode`, The `Color Scheme` is inspired by `.MD` file style under [Sublime Text 2.app] and Mou's Icon.

Screenshot:  
![Sublime-Preview.png](https://github.com/hzlzh/Mou-Theme/raw/master/Themes/Sublime-Preview.png)    

### Preview

_Both Code Mode & Live Preview Mode_

![Both.png](https://github.com/hzlzh/Mou-Theme/raw/master/CSS/Both.png)

## Contributions

`Star` or `Fork` to make this repo more and more wonderful~

## Credits
Created by @[hzlzh](https://twitter.com/hzlzh 'Contact me on Twitter') under [MIT] LICENSE


[Mou.app]: http://25.io/mou/
[Sublime Text 2.app]: http://www.sublimetext.com/
[Sublime.txt]:https://github.com/hzlzh/Mou-Theme/raw/master/Themes/Sublime.txt
[Sublime+.txt]:https://github.com/hzlzh/Mou-Theme/raw/master/Themes/Sublime+.txt
[GitHub-ReadMe.css]: https://github.com/hzlzh/Mou-Theme/raw/master/CSS/GitHub-ReadMe.css
[MIT]: http://rem.mit-license.org/

