# Puppeteer Recorder

[![Build Status](https://travis-ci.org/checkly/puppeteer-recorder.svg?branch=develop)](https://travis-ci.org/checkly/puppeteer-recorder)

![](src/images/recorder.png)
Puppeteer recorder is a Chrome extension that records your browser interactions and generates a 
[Puppeteer](https://github.com/GoogleChrome/puppeteer) script. This project is **very much in alpha stage**,
but does the following already:

- Records clicks and type events.
- Add waitForNavigation, setViewPort and other useful clauses. 
- Generates a Puppeteer script.
- Shows which events are being recorded.
- Copy to clipboard.
- Offers configuration options.

## Usage

- Click the icon and hit Record.
- Hit <kbd>tab</kbd> after you finish typing in an `input` element.
- Click links, inputs and other elements.
- Wait for full page load on each navigation. The icon will switch from ![](src/images/icon_rec.png) to ![](src/images/icon_wait.png).
- Click Pause when you want to navigate without recording anything. Hit Resume to continue recording. 
## Background

Writing Puppeteer scripts for scraping, testing and monitoring can be tricky. A recorder / code generator can be helpful,
even if the code isn't perfect. This project builds on other projects (see [disclaimer](#user-content-credits--disclaimer) 
below) but add extensibility, configurability and a smoother UI.

## Development

1. Run: `git clone https://github.com/checkly/puppeteer-recorder.git`
2. Build the project: `cd puppeteer-recorder && npm i && npm run dev`
2. Navigate to chrome://extensions
3. Make sure 'Developer mode' is checked
4. Click Load unpacked extension...
5. Browse to puppeteer-recorder/build and click Select

## Credits & disclaimer

Puppeteer recorder is the spiritual successor & love child of segment.io's 
[Daydream](https://github.com/segmentio/daydream) and [ui recorder](https://github.com/yguan/ui-recorder).

## License
MIT
