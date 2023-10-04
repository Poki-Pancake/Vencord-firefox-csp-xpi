# Vencord xpi

This is a custom fork and xpi build of Vencord for the firefox version of discord web.
Due to Mozilla's policy, the official firefox version of Vencord had some plugins and features taken away.
This fork brings them back.

Since I can't keep up with the official Vencord github repo, source code is availlable on the releases page and is only updated once in a while when I notice a feature breaking.
These builds were made for me in mind and keep in mind: **Use at your own risk. Any issues is not my problem**.

## Why?
- I can't live without vencord for firefox, because chromium version is laggy.
- I also can't live without CSP and shikicodeblocks

## How to install
1. Download the latest xpi from the release page.
2. In your firefox-based browser go to your `about:config`.
3. Set `extensions.langpacks.signatures.required` and `xpinstall.signatures.required` to `false`.
4. Go to the add-ons page.
5. Click the cog wheel on the corner then select the `Install add-on from file...`, then locate the downloaded xpi file.
6. On the installed add-on, go to its settings and set `Allow automatic updates` to `off`.

## How to build
1. Get Nodejs and pnpm.
2. Download the latest build source code from the release page then extract the tarball.
3. In the vencord directory perform the following commands:
```bash
$ pnpm i
$ pnpm buildWeb
```
4. Once compiled go to `dist/firefox-unpacked/`.
5. Compress all files in the `firefox-unpacked` directory into a zip file.
6. Rename the zip file and change the `.zip` into a `.xpi`.


