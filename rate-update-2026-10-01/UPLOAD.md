# Upload: drop "estimated" from the Chapter 35 period

RA's call, 2026-10-01: take the word out now rather than at the next app update. VA's published rates for
1 October 2026 to 30 September 2027 are $1,621, $1,281 and $939, and the file already carries exactly those.

`constants.json` in this folder is the live hosted file with one change, line 18:

    "label": "Oct 1, 2026 - Sep 30, 2027, estimated",   ->   "label": "Oct 1, 2026 - Sep 30, 2027",

`constants-live-before.json` is the hosted file as it stood before, kept so the change can be checked.
The app's built-in copy got the same change in college-tool e23e89a and ships with the next build.

## You upload, the standing rule for the rates repo

1. Open https://github.com/wegotthis-dotcom/wegotyou1776-rates/upload/main
2. Drag in `C:\dev\wegotyou1776\outbox\rate-update-2026-10-01\constants.json`
3. Commit message: Chapter 35 October 2026 period, drop estimated. Then Commit changes.
4. Give GitHub Pages a minute, then tell Code "check the rates upload" and it reads the hosted file back.

Every phone picks it up at its next launch; nothing else changes.
