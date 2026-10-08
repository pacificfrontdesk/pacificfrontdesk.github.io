# pacificfrontdesk.github.io

Root GitHub Pages site for the pacificfrontdesk org. It exists for one file:
`.well-known/apple-app-site-association`, which Apple only reads from the domain root.
It tells iOS which links on this domain open which app (universal links).

- Party Deck (`93NF8SSXQ6.com.olegnochka.partydeck`): `/partydeck/d#...` shared deck links.

`.nojekyll` is required, otherwise GitHub Pages skips the `.well-known` folder.
Each app's own pages stay in its own repo at `/<app>/`.
To add an app, add a `details` entry, push, and check Apple's cached copy:
`curl https://app-site-association.cdn-apple.com/a/v1/pacificfrontdesk.github.io`
