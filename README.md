# dgml.io

This repository serves [www.dgml.io](https://www.dgml.io). `index.html` (and
the other files at the repo root) are the site itself — what's actually
deployed and served to visitors.

## examples/

`index.html` links to [`examples/dgml-app-sample.html`](examples/dgml-app-sample.html)
via the "Try the App Sample" button. That file is a **copy** of
[`app-sample/dgml-app-sample.html`](https://github.com/dgml-io/dgml/blob/main/app-sample/dgml-app-sample.html)
from the [`dgml-io/dgml`](https://github.com/dgml-io/dgml) repo, vendored
here so the live site has something to link to and serve directly. The
source of truth for that sample lives in `dgml-io/dgml` — if it changes
there, re-copy it here to keep the site in sync.
