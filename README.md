# apko-helm-image-demo

An example of using [apko](https://github.com/chainguard-dev/apko)/[melange](https://github.com/chainguard-dev/melange) to create a fully reproducible container image based on alpine with Helm. We also get multi-arch and SBOM support.

- melange is used for creating apk package.
- we can then use apko to install that local package.
- we can do this for any arbitraty binary as well but it's not recommended if you want to do multi-arch build.

You can try it by pulling the image and see for yourself

```shell
docker pull ghcr.io/tuananh/apko-helm-image-demo:latest
```

## Goals

- [x] Fully reproducible build.
- [ ] Multi-arch support.
- [x] SBOM support.

## License

Copyright 2022 Tuan Anh Tran <me@tuananh.org>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.