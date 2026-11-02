# My Space portfolio

This is a simple static website for GitHub Pages, with a single JSON content file editable through Pages CMS.

## Important deployment note
This code assumes the site is hosted at the root of a domain. Use a repository named `YOUR_USERNAME.github.io`, or configure a custom domain. A project site at `username.github.io/repository` needs its absolute paths changed.

## Publishing
1. Create a public GitHub repository named `YOUR_USERNAME.github.io`.
2. Upload all contents of this folder, including `.pages.yml` (GitHub's web uploader may hide dotfiles; check that it is present).
3. GitHub repository Settings > Pages > Build and deployment > Deploy from a branch > main / (root).
4. Visit `https://YOUR_USERNAME.github.io` after deployment.
5. Open https://pagescms.org, sign in with GitHub, authorize the repository, and open `Website content`.
6. Add feed posts or projects in the JSON collections. Each block can be text, image, audio, video, or a YouTube/Vimeo embed. Save to commit changes to GitHub.
7. To use a domain you own, set it in GitHub Pages settings, then add the DNS records required by GitHub at your registrar. Wait for HTTPS to become available.

## Media note
The file picker in Pages CMS is configured as an image field; audio/video upload support depends on Pages CMS's media widget and accepted file types. If the editor rejects MP3/MP4 files, upload those files into the `media` folder in GitHub and paste their `/media/filename.mp3` paths into the `file` field. For larger videos, YouTube/Vimeo embeds are recommended. GitHub's browser upload limit is 25 MiB per file and normal Git has a 100 MiB hard file limit.

## Notes
- The timestamp is entered through Pages CMS; it is not automatically captured at publication.
- The project page deliberately has no header, just the date and content.
- The feed is a continuous scrolling page; for a very large archive, pagination or lazy loading would be a later enhancement.
- The website renders JSON as plain text and DOM nodes, not raw HTML.
