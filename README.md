# mathbrown.com

Homepage for Mr. Brown's course websites. Served by GitHub Pages at
https://mathbrown.com (DNS on Cloudflare).

- `index.html` — the whole homepage (styles + card physics inline).
  Cards dodge the cursor for 5 s, settle by 6 s. SPE4O never settles.
- `mhf4u/`, `mcr3u/`, `mth1w/` — forwarders to the course sites, which
  stay at their `quarkzebra.github.io/<CODE>/` URLs on purpose (board
  filtering may block this domain; the github.io URLs must keep working).
- `404.html` — forwards any capitalization of a course path, e.g. `/MHF4U`.
- `CNAME` — tells GitHub Pages this repo answers for mathbrown.com.

To add a course card: copy one of the `<a class="card">` blocks in
`index.html`, add a `--ac` accent for its `data-c` in both color-scheme
blocks, and add a forwarder folder + a line in the `404.html` map.
