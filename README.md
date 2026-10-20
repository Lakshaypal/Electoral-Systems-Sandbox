# Electoral Systems Sandbox — Hobby Visualisation Project

A personal learning project built around election-synchronisation scenarios. It explores React dashboards, timelines, charts and an optional Gemini-generated explanation panel.

**Hobby prototype:** numerical assumptions are hard-coded demonstrations, not validated policy forecasts or an official election dataset. The interface is intended for experimenting with visualisation and application state.

## Screens

- Overview and election-cycle timelines.
- Illustrative financial, administrative and governance comparisons.
- A scenario-selection wizard and optional AI explanations.
- Reference links and contextual constitutional information.

The scenario wizard currently keeps its own local state; it is not a fully integrated policy-simulation engine. Constitutional text is prototype content rather than legal guidance.

## Run locally

Use Node.js 20+:

```sh
git clone https://github.com/Lakshaypal/Electoral-Systems-Sandbox.git
cd Electoral-Systems-Sandbox
npm ci
npm run dev
```

Vite starts on port 3000. To build a static bundle:

```sh
npm run build
npm run preview
```

The optional AI service currently requests `gemini-3-pro-preview`. Without a key, the charts and scenario calculations still run. The existing frontend integration embeds a configured key in the browser bundle; a public AI deployment needs a server-side proxy. Never put a private API key in a publicly served build.

## Stack

React, TypeScript, Vite, Recharts, Lucide and the Google GenAI SDK. This is a hobby/demo repository, separate from the research projects on this profile.
