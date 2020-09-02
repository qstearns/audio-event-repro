# Svelte SSR Event Reproduction

This project demonstrates an issue with Svelte events on Firefox wherein the expected events don't fire when binding components to values in audio elements.

## Relevant source

The code demonstrating the issue lives at [the index route](./src/routes/index.svelte)

## Running

Run `yarn && yarn dev` from the repo root and then visit localhost:3000 from Firefox and reload the page. You'll see that the audio duration loads as zero on the second instance of the page load.

Furthermore, you'll see that the `on:durationchange` handler never fires on the second page load.

