# Hibernate Tabs, Windows, and Sessions

HTWS is a memory-saving Chromium extension created because native tab suspension
did not reduce memory reliably enough for the workflow it was meant to solve. It
saves a complete local restore record and then closes the selected tabs,
windows, or session so Chromium can reclaim their live page resources. Users can
restore their tab order, pins, groups, names, and active state later.

This repository publishes the HTWS homepage, privacy policy, and support page
for the Chrome Web Store listing:

- [Homepage](https://ilobaak.github.io/htws-extension-site/)
- [Privacy policy](https://ilobaak.github.io/htws-extension-site/privacy.html)
- [Support](https://ilobaak.github.io/htws-extension-site/support.html)

HTWS stores hibernation records locally. It does not use analytics, advertising,
or a developer-operated server. Exact per-tab memory savings are not reported
because stable extension APIs do not expose reliable measurements.

## Measured memory savings

In a controlled 24-run Brave benchmark on Windows 10, HTWS released 11.7 to 13.2
times more median process working set than native tab discard across workloads
from 10 to 100 tabs. Read the complete
[benchmark report](https://ilobaak.github.io/htws-extension-site/assets/HTWS-memory-savings-benchmark.pdf)
for the raw results, graphs, method, and limitations. Actual savings vary by
website, browser version, system, and time after hibernation.

The generated `assets/icon-128.png` comes from the reviewed extension icon. Run
`npm run store:assets` after changing that icon or any store screenshot.
