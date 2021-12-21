# rootofpi.co.uk

Welcome! Here lies some Basic information about Michael Pearce, a software engineer from the United Kingdom.
A static site quickly and easily generated with [Hugo](https://gohugo.io/getting-started/quick-start/), styled with a modified version of the [Timeline](https://github.com/s4n7h0/hugo-theme-timeline) theme.

## Development

A brief list of noteable reminders for future reference

- Install Hugo (see the [Hugo Quickstart Guide](https://gohugo.io/getting-started/quick-start/))
- `hugo new books/bemorepirate.md`
- `hugo server -D` (run the server with Draft mode enabled, which should rebuild as changes are made and saved)
- View the site locally at http://localhost:1313/ (unless stated otherwise in the terminal!)
- `hugo -D` (Build the static pages, output should go to ./public/ by default)

### Adding Themes

(As per [Hugo Quickstart Guide](https://gohugo.io/getting-started/quick-start/)) First, download the theme from GitHub and add it to your site’s themes directory:

- `git submodule add [<url>] themes/[<name of theme>]`

For example:

- `git submodule add https://github.com/s4n7h0/hugo-theme-timeline themes/timeline`

You may choose to fork a repository for a theme to make your own changes or additions: 

- `git submodule add https://github.com/pearcem0/hugo-theme-timeline themes/timeline`

## Deployment

Currently deployed to AWS (Amazon Web Services).

- Static files stored in Amazon S3 with Static website hosting enabled.
- DNS and HTTPS redirection configured with [CloudFlare](https://support.cloudflare.com/hc/en-us/articles/360037983412-Configuring-an-Amazon-Web-Services-static-site-to-use-Cloudflare).

### Uploading files to S3

Something _like_...
`aws s3 cp public/ s3://<bucket name> --recursive --profile <profile name>`

## Errors or Omisions?

If you spot something wrong, or have something to add feel free to create a Pull Request.