# ReDI School Workshop App Template

A minimal React, TypeScript, and Vite starter for workshop app ideas. The app displays **Hello World**.

## Customize for an app idea

When forking this repository, fill in [APP_BRIEF.md](APP_BRIEF.md) with the app idea, main user journey, and demo acceptance criteria. The agent follows the shared defaults in [AGENTS.md](AGENTS.md); record any explicit participant overrides in the brief.

## Install prerequisites

To run the app, you need **Node.js 24 LTS**, **npm** (included with Node.js), and a web browser. Install **Git** to clone the repository and save changes. React, TypeScript, and Vite are installed locally by `npm ci`; they do not need separate system-wide installations.

Complete this setup before the workshop:

| System | Node.js and npm | Git | Terminal to use |
| --- | --- | --- | --- |
| macOS | On the [Node.js download page](https://nodejs.org/en/download), select Node 24 LTS and macOS, then download and run the `.pkg` installer. | Run `xcode-select --install` and follow the prompts. See the [macOS Git guide](https://git-scm.com/install/mac). | Terminal |
| Linux | Follow the [nvm installation guide](https://github.com/nvm-sh/nvm#installing-and-updating), reopen your terminal, then run `nvm install 24` and `nvm use 24`. See also the [Node/npm installation guide](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm/). | Use your distribution's package manager: for Ubuntu/Debian, run `sudo apt update` followed by `sudo apt install git`. See the [Linux Git guide](https://git-scm.com/install/linux) for other distributions. | Your usual terminal |
| Windows | On the [Node.js download page](https://nodejs.org/en/download), select Node 24 LTS and Windows, then download and run the `.msi` installer with the default settings. | Install [Git for Windows](https://git-scm.com/install/windows) with the default settings. | Command Prompt |

Reopen your terminal after installing, then verify:

```sh
node --version
npm --version
git --version
```

Node should print `v24.x.x`; npm and Git should each print a version number. If a command is not found, check that installation finished and reopen the terminal.

If you already use nvm on macOS or Linux, run `nvm install` and `nvm use` inside this repository to select the version in `.nvmrc`.

## Run locally

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
