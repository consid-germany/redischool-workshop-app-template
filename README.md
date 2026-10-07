# ReDI School Workshop App Template

A minimal React, TypeScript, and Vite starter for workshop app ideas. The app displays **Hello World**.

## Run locally

Install Node.js 24 LTS (which includes npm) and Git before starting.
If you use nvm, run `nvm install` and `nvm use` inside this repository to select the version in `.nvmrc`.

1. Clone this repository using its Git URL, then open a terminal in the cloned folder.
2. Install the dependencies:

   ```sh
   npm ci
   ```

3. Start the development server:

   ```sh
   npm run dev
   ```

4. Open the local URL printed in the terminal, usually http://localhost:5173.
   You should see **Hello World**. Edits to `src/App.tsx` update the page automatically.

Press `Ctrl+C` in the terminal to stop the server.

## Check and build

```sh
npm run lint
npm run build
```

The build command checks TypeScript and creates the production files in `dist/`.
To view the built app locally, run `npm run preview` after building and open the URL printed in the terminal.
