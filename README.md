# Pedalwise support

Public support, privacy and terms pages for Pedalwise. The app source lives in a separate private repository.

## Cloudflare deployment

Same setup as the Shift Calendar support site: Cloudflare Pages with Git integration, build command `npm run build`, output `dist`, Node 22+. Pages project name `pedalwise`, custom domain `pedalwise.jelluna.com`. No server, database, analytics or secrets.

```sh
npm run build
npm run dev
```

The build copies an explicit list of public files into `dist/` and fails on broken local links or fragments.
