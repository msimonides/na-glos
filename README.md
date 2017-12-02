# Experimenting with speech command recognition in a browser

The experiment uses `webkitSpeechRecognition` to repeatedly listen to voice
commands and execute them. This is nothing new, see below for ready made solutions.

Here I have added feedback, so that the user knows what is happening, and improved
responsiveness. Responsiveness may sometimes become an issue when the final recognition
result is delivered with a noticeable delay, up to several seconds (this may be due to
poor microphone perhaps). The interim results are hovever often good enough so that the
last interim result is used if there are no new results within one second.

## Testing

[Open the demo](https://msimonides.github.io/na-glos/) in Chrome, allow microphone
access when prompted and say "next page", "down" or "forward" to scroll down and
"previous page", "up" or "back" to scroll up.

## Similar work

- [artyom.js](https://sdkcarlos.github.io/sites/artyom.html)
- [annyang](https://www.talater.com/annyang/)

Actually my code is based on the ideas in these two libraries.

## License

Copyright 2017 Marcin Simonides, licensed under the [MIT License](LICENSE)
