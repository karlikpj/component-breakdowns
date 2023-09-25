---
title: Getting Started for Developers
nav_label: Getting Started for Developers
nav_order: 1000000
---

# Developer Setup

### Install Node

Ensure that you have Node.js installed.
Current Requirment: Gallium LTS (Long-Term Support).

Open your Terminal application and a Terminal window. Check to see if you have Node installed with `node -v`.

If you don’t have Node, install it from [Node Version Manager](https://github.com/nvm-sh/nvm) or [Node.js](https://nodejs.org/en/download/).

#### Node Version Manager (recommended)

1. Visit the official NVM repository on GitHub: https://github.com/nvm-sh/nvm
2. Follow the installation instructions specific to your operating system.
3. Once installed, close and reopen your terminal or command prompt to ensure NVM is properly set up. `nvm -v`
4. Install Node.js `nvm install lts/gallium`
5. Change it to the preferred mode version `nvm use lts/gallium`
6. Verify that the preferred version is set `node -v`

#### Download

1. Visit the official Node.js website: https://nodejs.org
2. On the Node.js website, click on the "Downloads" tab located in the top menu.
3. Look for the LTS (Long-Term Support) version section. It typically contains the recommended version for most users.
4. Within the LTS section, check if Gallium is listed as an available option. Gallium is a codename used for specific LTS releases.
5. If Gallium is listed, click on the corresponding download button to initiate the download.
6. Choose the appropriate installer for your operating system (Windows, macOS, or Linux) and click on the download link.
7. Once the download is complete, locate the downloaded installer file on your computer.
8. Run the installer and follow the on-screen instructions to complete the installation process.
9. After the installation is finished, open a terminal or command prompt and type node -v to verify that Node.js is installed correctly.

### Install a package manager

1. npm (recommended):

Open your terminal or command prompt.
npm is the default package manager that comes bundled with Node.js, so there is no need to download it separately.
To check the version of npm installed, run the command

```bash
npm --version.
```

2. Yarn

Open your terminal or command prompt. Run the following command to download and install Yarn globally:

```bash
npm install -g yarn
```

This command will use npm to download and install Yarn globally on your system. Once the installation is complete, you can verify it by running the command `yarn --version`.

3. PNPM:

Open your terminal or command prompt. Run the following command to download and install PNPM globally:

```bash
npm install -g pnpm
```

After the installation, you can verify it by running the command `pnpm --version`.
