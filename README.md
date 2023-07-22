
<div align="center">
  <h3 align="center">
    ZeroSlides
  </h3>

  <p align="center">
    My slides template powered by <a href="https://sli.dev/"> slidev </a>
  </p>
</div>

## Getting Started


### Prerequisites

- npm / node.js
```bash
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash
$ nvm install 18
$ nvm use 18
```

- slidev

```bash
$ npm i -g @slidev/cli @slidev/theme-default
```

### Installation

- Basic
```bash
$ git clone https://github.com/Zerokei/ZeroSlides.git
$ cd ZeroSlides
$ npm install
```

- Export pdf
```bash
$ node_modules/.bin/playwright install-deps
```

## Usage

```bash
$ npm run dev # start dev server
$ npm run export # export to pdf
$ npm run build # build the project and generate the html code
```

## Roadmap

- [x] Export pdf
- [ ] Static Hosting
- [ ] Cover