# YouTube Shorts Player Bypass

[![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](http://unlicense.org/)

A Chrome extension that redirects YouTube Short URLs to the regular video player.

## Purpose

I got annoyed with YouTube's Shorts player, and I didn't want to manually modify the video URLs to load the regular player anymore.

## Method

The extension uses a naïve approach. It assumes that the short is accessed with a URL of the following format:

```
https://www.youtube.com/shorts/<video-id>
```

It then replaces the URL with:

```
https://www.youtube.com/watch?v=<video-id>
```

This does not work when the Shorts page is accessed from some of YouTube's UI elements, but a page refresh should work in that case.

Feedback and/or patches that improve on this approach are welcome.

## Installing

The extension is currently not available on the [Chrome Web Store](https://chromewebstore.google.com/), it has to be installed manually.

1. Save the extension to your device.
2. Follow the instructions under the section **Load an unpacked extension** [here](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world).