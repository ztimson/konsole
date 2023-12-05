<!-- Header -->
<div id="top" align="center">
  <br />
  
  <!-- Logo -->
  <img src="https://git.zakscode.com/repo-avatars/5821977def5119fa0d4ea37698e849e07d3fab53e7ed7457af55d25ea8709ea0" alt="Logo" width="200" height="200">

  <!-- Title -->
  ### Konsole
  
  <!-- Description -->
  Experimental Web Based CLI

  <!-- Repo badges -->
  [![Version](https://img.shields.io/badge/dynamic/json.svg?label=Version&style=for-the-badge&url=https://git.zakscode.com/api/v1/repos/ztimson/konsole/tags&query=$[0].name)](https://git.zakscode.com/ztimson/konsole/tags)
  [![Pull Requests](https://img.shields.io/badge/dynamic/json.svg?label=Pull%20Requests&style=for-the-badge&url=https://git.zakscode.com/api/v1/repos/ztimson/konsole&query=open_pr_counter)](https://git.zakscode.com/ztimson/konsole/pulls)
  [![Issues](https://img.shields.io/badge/dynamic/json.svg?label=Issues&style=for-the-badge&url=https://git.zakscode.com/api/v1/repos/ztimson/konsole&query=open_issues_count)](https://git.zakscode.com/ztimson/konsole/issues)

  <!-- Links -->
  ---
  <div>
    <a href="https://git.zakscode.com/ztimson/konsole/wiki" target="_blank">Documentation</a>
    • <a href="https://git.zakscode.com/ztimson/konsole/releases" target="_blank">Release Notes</a>
    • <a href="https://git.zakscode.com/ztimson/konsole/issues/new?template=.github%2fissue_template%2fbug.md" target="_blank">Report a Bug</a>
    • <a href="https://git.zakscode.com/ztimson/konsole/issues/new?template=.github%2fissue_template%2fenhancement.md" target="_blank">Request a Feature</a>
  </div>

  ---
</div>

## Table of Contents
- [Konsole](#top)
  - [About](#about)
    - [Built With](#built-with)
  - [Demo](#demo)
  - [Setup](#setup)
    - [Development](#development)
  - [License](#license)

## About

This is an experimental project to simulate a bash console inside the webbrowser. It is ment to be highly configurable & extendable like a real CLI.

Programs can be added to the environment by extending the global `cli` dictionary like so:  
```
window.cli['echo'] = {
    autocomplete: () => {
        return [];
    },
    help: () => {
        return 'Output text to console';
    },
    run: args => {
        return args.join(' ');
    }
}
```

Everything is written in vanilla JS so it can be easily ported.

### Built With
[![HTML](https://img.shields.io/badge/HTML-FFFFFF?style=for-the-badge&logo=html5)](https://developer.mozilla.org/en-US/docs/Glossary/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-000000?style=for-the-badge&logo=javascript)](https://javascript.com/)

# Demo

Download & open [index.html](./index.html)

## Setup

<details>
<summary>
  <h3 id="development" style="display: inline">
    Development
  </h3>
</summary>

#### Instructions
1. Open `index.html` & edit away

</details>

## License
Copyright © 2023 Zakary Timson | Available under MIT Licensing

See the [license](./LICENSE) for more information.
