## About

Do you need to convert your JS to strictly uppercase or lowercase? No problem. This is a web app that converts it for you.

https://arinerron.github.io/case-insensitive-xss/index.html

## How does it work?

Basically, it JSF\*ck-encodes `eval(decodeURIComponent(...))` where `...` is your JavaScript, and URL encodes the other uppercase/lowercase characters.

## Does it always work?

Yes, as long as the target app's CSP whitelists `eval`.
