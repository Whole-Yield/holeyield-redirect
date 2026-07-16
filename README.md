# holeyield.com redirect

`holeyield.com` is the defensive typo registration for `wholeyield.com`
(registered 2016-12-10, two days after the real one). This repo does nothing but
bounce web traffic to the real domain.

`index.html` and `404.html` are identical on purpose: the 404 copy is what makes
`holeyield.com/some/path` forward to `wholeyield.com/some/path` instead of dying
on a GitHub 404. Keep them in sync.

## Do not touch its MX records

This domain has **live Google Workspace MX records** and is catching mistyped
mail today. This repo only ever affects A records and the web side. If you are in
the Namecheap panel for holeyield.com, leave the MX rows alone.

## Publishing

GitHub Pages, `main` / root. `CNAME` holds `holeyield.com`. The apex A records
are the same four GitHub Pages addresses as the other sites.
