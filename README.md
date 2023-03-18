# Yew Example
[![Continuous integration](https://github.com/JRedrupp/yew-example/actions/workflows/CI.yml/badge.svg?branch=master)](https://github.com/JRedrupp/yew-example/actions/workflows/CI.yml)[![Continuous deployment](https://github.com/JRedrupp/yew-example/actions/workflows/CD.yml/badge.svg)](https://github.com/JRedrupp/yew-example/actions/workflows/CD.yml)

This is a simple example of a Yew application. It is a simple counter that can be incremented and decremented.
Guide Follow the [Yew Guide](https://yew.rs/docs/getting-started/build-a-sample-app) to build this example.

## Build
To build this example, run the following command in this directory:
```bash
trunk serve
```

## Access from Web
To access this example from the web, open the following URL in your browser:
https://jredrupp.github.io/yew-example/

## CI / CD
This example uses GitHub Actions to build and deploy the example to GitHub Pages. The following files are used:
- [CI.yml](.github/workflows/CI.yml): Builds the example and runs tests.
- [CD.yml](.github/workflows/CD.yml): Builds the example and deploys it to GitHub Pages.

Referenced (plippe)[https://plippe.github.io/blog/2021/07/12/rust-wasm-github.html] as a guide for setting up CI/CD.

Note: In order to deploy to GitHub Pages, you must create a GitHub token and add it to the repository secrets.
The Build command must have the `--public-url /${{ github.event.repository.name }}` flag set so the assets are loaded.

## License
MIT License

Copyright (c) 2023 Jake Redrupp

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.