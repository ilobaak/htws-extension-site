# HTWS Public Site

This directory contains the public homepage, privacy policy, and support page
prepared for the Chrome Web Store listing.

Publish it from a separate public GitHub repository, such as
`ilobaak/htws-extension-site`, so the extension source repository can remain
private. Enable GitHub Pages from the repository's default branch and verify
that all three pages are available over HTTPS before entering their URLs in the
Chrome Web Store dashboard.

The generated `assets/icon-128.png` comes from the reviewed extension icon. Run
`npm run store:assets` after changing that icon or any store screenshot.
