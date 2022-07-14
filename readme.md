Example of deploying a Vite + `vite-plugin-ssr` app to [Vercel](https://vercel.com/), using Vercel's [FileSystem API](https://vercel.com/docs/file-system-api/v1).

While/after adding your Git repository to Vercel, set the following in Vercel's web UI:
 1.  Set `FRAMEWORK PRESET` to Other.
 1. Add a new environment variable named `ENABLE_FILE_SYSTEM_API` and set its value to `1`.

Highlights:

 - See [`vercel/deploy.sh`](vercel/deploy.sh).
 - See the [package.json](package.json)'s build scripts `package.json#scripts['vercel-build']` and `package.json#scripts.build`.
 - See the [package.json](package.json)'s dev script `package.json#scripts.dev`: we use Vite's development server for improved DX.
