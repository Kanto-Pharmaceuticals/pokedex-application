# Pokedex Application

The Pokédex is a Full MERN Stack Application to catalogue and provide data on all the species of Pokémon featured in the video game, anime and manga series.

## Getting Started with Development

This repo uses yarn as it's package manage and for launching scripts for development and deployment. The package `concurrently` is used to run multitple commands concurrently, as in the case of `yarn dev`.

```
yarn server
```

This command will set the current working directory(`--cwd`) to the `./backend` folder will running the `server` command. This command will chain to the backend `package.json`'s own `server` command.

```
yarn client
```

Similar to above, the current working directory is also changed, but to `./frontend` instead to invoke the frontends `start` command.

```
yarn dev
```

Uses `concurrently` to run both `yarn server` and `yarn client` concurrently for development work.

## Important

This repository was created as submodule of the [Pokedex](https://github.com/Kanto-Pharmaceuticals/pokedex) with the intention of re-using it's code for scaffolding other projects. It is important to have some knowledge of working with `git` and `submodules` in CLI in order to avoid breaking pointer references.
