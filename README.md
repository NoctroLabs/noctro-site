# noctro.co.uk

The Noctro Labs studio site. It's plain static HTML with no build step: `index.html`, `404.html`, `nestwise/privacy/`, `nestwise/support/`, `assets/` and `CNAME`.

The App Store URLs for Nestwise are:
- Privacy: https://noctro.co.uk/nestwise/privacy/
- Support: https://noctro.co.uk/nestwise/support/

## Preview locally

    python3 -m http.server 8787

## Deploy (GitHub Pages, same setup as slabd.app)

1. Push this folder to a repo such as `NoctroLabs/noctro-site`.
2. In the repo, go to Settings → Pages → Deploy from branch `main` / root.
3. Add these DNS records for `noctro.co.uk` at your registrar:
   - Four `A` records on `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - A `CNAME` record on `www` pointing to `noctrolabs.github.io`
4. Once the certificate is issued, tick "Enforce HTTPS".

## Editing

- When Nestwise goes live, change its "Coming soon to the App Store" text to an App Store link. It appears in the app card and the roadmap.
- When an app in the lab is announced, replace one of the `.slot.lab` roadmap tiles with a `.slot.live` tile.
- The email aliases are `hello@` (studio), `slabd@` and `nestwise@` (app support), all at noctro.co.uk.
- Phone screenshots are in `assets/shots`. Nestwise shots come from the simulator's `-demo` mode, which uses a fictional family. Never publish real family data.
