<p align="center">
  <a href="https://liveblocks.io#gh-light-mode-only">
    <img src="https://raw.githubusercontent.com/liveblocks/liveblocks/main/.github/assets/header-light.svg" alt="Liveblocks" />
  </a>
  <a href="https://liveblocks.io#gh-dark-mode-only">
    <img src="https://raw.githubusercontent.com/liveblocks/liveblocks/main/.github/assets/header-dark.svg" alt="Liveblocks" />
  </a>
</p>

# Notification Settings

<p>
  <a href="#">
    <img src="https://img.shields.io/badge/live%20preview-message?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTE2Ljg0OSA0Ljc1SDBsNC44NDggNS4wNzV2Ny4wMDhsMTItMTIuMDgzWk03LjE1IDE5LjI1SDI0bC00Ljg0OS01LjA3NVY3LjE2N2wtMTIgMTIuMDgzWiIgZmlsbD0iI2ZmZiIvPjwvc3ZnPg==&color=333" alt="Live Preview" />
  </a>
  <a href="https://codesandbox.io/s/github/liveblocks/liveblocks/tree/main/examples/nextjs-tiptap">
    <img src="https://img.shields.io/badge/open%20in%20codesandbox-message?style=flat&logo=codesandbox&color=333&logoColor=fff" alt="Open in CodeSandbox" />
  </a>
  <img src="https://img.shields.io/badge/react-message?style=flat&logo=react&color=0bd&logoColor=fff" alt="React" />
  <img src="https://img.shields.io/badge/next.js-message?style=flat&logo=next.js&color=07f&logoColor=fff" alt="Next.js" />
  <img src="https://img.shields.io/badge/tiptap-message?style=flat&color=7bf" alt="Tiptap" />
</p>

This example shows how handle notification settings for users in [Liveblocks](https://liveblocks.io), in a collaborative text editor built with [Tiptap](https://tiptap.dev/), [NextAuth](https://next-auth.js.org/), and [Next.js](https://nextjs.org/).

With [Liveblocks Notifications](https://liveblocks.io/notifications), each user can choose whether they should receive notifications on different channels, for example Email, Slack, Teams. This example highlights how to create a settings panel for adjusting which notification webhooks should be triggered for the current user.

<img src="https://raw.githubusercontent.com/liveblocks/liveblocks/main/.github/assets/examples/text-editor.png" width="536" alt="Collaborative Text Editor" />

## Getting started

Run the following command to try this example locally:

```bash
npx create-liveblocks-app@latest --example nextjs-notification-settings --api-key
```

This will download the example and ask permission to open your browser, enabling you to automatically get your API key from your [liveblocks.io](https://liveblocks.io) account.

Before running the project, make sure to create your [NextAuth secret](https://next-auth.js.org/configuration/options#nextauth_secret) first:

```bash
npx auth secret
```

### Manual setup

<details><summary>Read more</summary>

<p></p>

Alternatively, you can set up your project manually:

- Install all dependencies with `npm install`
- Create an account on [liveblocks.io](https://liveblocks.io/dashboard)
- Copy your **secret** key from the [dashboard](https://liveblocks.io/dashboard/apikeys)
- Create an `.env.local` file and add your **secret** key as the `LIVEBLOCKS_SECRET_KEY` environment variable
- Run `npx auth secret` to create a [NextAuth secret](https://next-auth.js.org/configuration/options#nextauth_secret).
- Run `npm run dev` and go to [http://localhost:3000](http://localhost:3000)

</details>

### Deploy on Vercel

<details><summary>Read more</summary>

<p></p>

To both deploy on [Vercel](https://vercel.com), and run the example locally, use the following command:

```bash
npx create-liveblocks-app@latest --example nextjs-notification-settings --vercel
```

This will download the example and ask permission to open your browser, enabling you to deploy to Vercel.

Make sure to generate a [NextAuth secret](https://next-auth.js.org/configuration/options#nextauth_secret) and add it to the `AUTH_SECRET` environment variable.

</details>

### Develop on CodeSandbox

<details><summary>Read more</summary>

<p></p>

After forking [this example](https://codesandbox.io/s/github/liveblocks/liveblocks/tree/main/examples/nextjs-notification-settings) on CodeSandbox, create the `LIVEBLOCKS_SECRET_KEY` environment variable as a [secret](https://codesandbox.io/docs/secrets).

Make sure to generate a [NextAuth secret](https://next-auth.js.org/configuration/options#nextauth_secret) and add it to the `AUTH_SECRET` environment variable.

</details>
