<h1 align="center">
    <img src="/docs/img/logo.png" alt="Logo">
</h1>

<p align="center">
    <a href="https://vuejs.org/"><img alt="VueJS 2" src="https://img.shields.io/badge/Vue-v2-98b23c.svg"/></a>
    <a href="https://nodejs.org/en/"><img alt="NodeJS v10" src="https://img.shields.io/badge/Node-v10.x-43b23c.svg"/></a>
    <a href="https://github.com/Simonwep/vue-cloudfront/tree/master"><img alt="Stable Branch" src="https://img.shields.io/badge/Stable%20Branch-master-3FB27F.svg"/></a>
    <a href="https://github.com/Simonwep/vue-cloudfront/tree/dev"><img alt="Development Branch" src="https://img.shields.io/badge/Dev%20Branch-dev-3eacb2.svg"/></a>
    <img alt="Product state: Alpha" src="https://img.shields.io/badge/State-pre--alpha-3c71b2.svg"/>
    <a href="https://www.patreon.com/simonwep"><img alt="Support me" src="https://img.shields.io/badge/Patreon-support-553cb2.svg"></a>
</p>


Vue Cloudfront is a blazing fast, standalone PWA cloudfront, basically for self-hosting purposes. 
Currently the only backend-solution is the official [vue-cloudfront-api](https://github.com/Simonwep/vue-cloudfront-api) which is a fully-featured RESTful api. This project is and will always be open source, anybody can contribute to it - it should, and hopefully will be, a massive improvement regarding cloud solutions in contrast to google-drive and drop-box. The project is currently in the **alpha** phase.

For anyone who wants some guidance, feel free to contact me on Discord: `Simon#6765`

<h3 align="center">
   <b><a href="https://vue-cloudfront.com/">Try out the fully featured demo! (user/pass: admin/admin)</b>
</h3>

## Features

Vue-cloudfront currently has full desktop and touch support (tablets / notebooks with touch support),
but no support for mobile devices (but [it's in progress](https://github.com/Simonwep/vue-cloudfront/tree/mobile-support))

All modern browsers like Chrome, Firefox, Opera, Edge and Safari are supported. See [.browserslistrc](/.browserslistrc) for further details.
IE support is and will never be in consideration.

#### Vue Cloudfront - unique features
* 100% Offline support (Navigation and searching) - via [localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage).
* Ultra lightweight, only '~ 60kb' js and '~ 20kb' css! (both gzipped).
* Realtime synchronization between sessions.
* Blazing fast with local caching: Average server response time: '~ 30ms' / Client-side rendering time: '~ 1.5s'.
* Installable - [Install it on your desktop](https://developers.google.com/web/progressive-web-apps/desktop) (Currently only supported by Chrome 70+ under Linux, Windows and Chrome OS).
* Modern Vue frontend with material-design - easy to design and customize.
* Simply structure and just a few dependencies.

#### File Management
* GridView with small file previews and draggable tiles.
* ListView with sortable columns and more details.
* Easy drag 'n drop as well as selection functionality.
* Files and folders can be marked _(for example to have quick access to them)_.
* Custom colors and color picker for faster content recognition.
* Almost no latency during a search.
* Copy, cut and move files and folders like on your notebook.
* Simultaneous uploads with a neat upload popup to control and see current uploads.
* Download entire directorie structures as zip file.

#### General
* Tooltips and introduction boxes to quickly understand how everything works.
* 29 Shortcuts, everything can also be done via a keyboard. No mouse at all required.
* File preview (currently only for images, videos, audio files, fonts and PDF).
* Search in your cloud and get results under '< 500ms'.
* Specify your search with file-type, size-range and more.

## Benchmarks
As a comparison, I compared the upload stats with these from google drive.
All benchmarks are made with an upload speed of `9.89 Mbit/s` / a ping of `~9ms`

##### Upload of node_modules (26.3MB, 7.567 Files and 590 Folders)
* Vue Cloudfront: `~40 Seconds` / `2 Requests`
* Google Drive: `~39 Minutes` / `9644 Requests`

##### Upload of one file (123MB)
* Vue Cloudfront: `~1 Minute and 53 Seconds` / `1 Request`
* Google Drive: `~2 Minutes and 10 Seconds` / `176 Requests`

##### Lighthouse analysis
![Lighthouse result](https://user-images.githubusercontent.com/30767528/51075890-f2239d00-1691-11e9-93e5-a34daad6fb0c.png)


## Documentation and table of contents

Currently and as already mentioned, this project is in its alpha phase. If all features and issues which I currently face are fixed and implemented, I will start to document stuff like config files, etc. Anyway the code is _(hopefully)_ well-equipped with comments.

Vue Cloudfront has been (so far) only deployed on an 'debian 9.5' instance, and I myself only work on Windows machines so the installation instructions on MacOS are only _assumed_ and based on these on Linux - If there are any issues/suggestions feel free to open a PR / Issue.

### Installation
* [Installing on MacOS](/docs/installation/mac.md)
* [Installing on Linux](/docs/installation/linux.md)
* [Installing on Windows](/docs/installation/windows.md)
* [Production setup](/docs/installation/production-setup.md)

See our [configuration docs](/docs/config.md) for further tweaks.

#### Vue Cloudfront stack
* [Vue as Framework](https://vuejs.org/)
* [Vuex as state management solution](https://vuex.vuejs.org/)
* [Fontawesome-free for fancy icons](https://fontawesome.com/)
* [Normalize.css for more consistently style](https://necolas.github.io/normalize.css/)
* [Selectionjs to provide selection experience like on your desktop](https://github.com/Simonwep/selection)
* [Service Worker to provive offline experience](https://developers.google.com/web/fundamentals/primers/service-workers/)
* [PWA](https://developers.google.com/web/progressive-web-apps/)

#### Vue Cloudfront-api stack
* [Express as Framework](https://expressjs.com/)
* [Mongoose as database API](https://mongoosejs.com/)
* [MongoDB as database](https://www.mongodb.com/)
* [PM2 as load balancer](https://pm2.io)

##### Current branches
* [mobile-support](https://github.com/Simonwep/vue-cloudfront/tree/mobile-support) - (in progress) Mobile and general touch-support.
* [settings](https://github.com/Simonwep/vue-cloudfront/tree/settings) - (in progress) Additional home-tab with user-settings.
* [realtime-sync](https://github.com/Simonwep/vue-cloudfront/tree/realtime-sync) - Realtime synchronization between sessions.
* [history](https://github.com/Simonwep/vue-cloudfront/tree/history) - (aborted) Additional home-tab with a temporary, visual log of all your actions.
* [terminal](https://github.com/Simonwep/vue-cloudfront/tree/terminal) - (aborted) Additional home-tab with a full functional terminal like bash.


## Screenshots
Checkout the [demo](https://vue-cloudfront.com/) the get an extensive view!
![screenshot 80](https://user-images.githubusercontent.com/30767528/52915771-4a287180-32d8-11e9-9a81-9d3dad00f3e2.png)
![screenshot 81](https://user-images.githubusercontent.com/30767528/52915772-4a287180-32d8-11e9-9b16-794e927a24c6.png)
![screenshot 82](https://user-images.githubusercontent.com/30767528/52915773-4a287180-32d8-11e9-9af9-3cc3b586b0d1.png)
![screenshot 83](https://user-images.githubusercontent.com/30767528/52915774-4a287180-32d8-11e9-8e59-a4a3ab8ba57b.png)
![screenshot 84](https://user-images.githubusercontent.com/30767528/52915775-4a287180-32d8-11e9-9f33-8099e3c20178.png)
![screenshot 73](https://user-images.githubusercontent.com/30767528/52915776-4ac10800-32d8-11e9-8f78-f942f878e3f0.png)
![screenshot 74](https://user-images.githubusercontent.com/30767528/52915777-4ac10800-32d8-11e9-9d01-d99c7e8f1132.png)
![screenshot 77](https://user-images.githubusercontent.com/30767528/52915778-4ac10800-32d8-11e9-923d-5093d10bcd91.png)
