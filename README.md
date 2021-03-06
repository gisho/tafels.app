# Tafels.App

A simple game to teach kids basic math (multiplication tables, additions, etc.)

Made with:

- `svelte` and `sapper`🎆
- nice animations and page transitions 🍡
- service workers 🌐
- web Audio with Howler 🎺
- UI + colors based on book Refactoring UI 🎉

## Development

```sh
yarn dev
```

## Build

```sh
yarn export
```

## Deploy

```sh
git push # 😸
```

## About Sapper and Svelte

Needs some polishing here and there (lots of bug fixes with every new version) but in general it's pretty cool. Less code & a faster user experience. Built-in animations are a big win (always a pain with React) and the routing solution that Sapper offers (also for SPA's) is a godsend compared to React Router.

I think it's very hard to beat Next.js' developer experience. The Next team has been really killing it with new features lately. So I think Sappers appeal comes mainly from... Svelte 😆.

But there are a few things I like: you can just use <a href=... and it (more of less) just works. No need for special <Link to /> components. Code splittings works well, and with Svelte being so small, you end up with tiny bundle sizes. However I did have to add/create a loader myself for when the Javascript was being loading (it's the blue top bar). This seems like something the framework should add add out of the box, otherwise users on slow connections might be wondering why their click on a link doesn't do anything.

Developing with Service Workers turned on (i.e. in dev mode) really works well with Sapper too, not sure how they're doing that!

## PWA tips

- Tried using pwacompat but it wasn't doing anything for me on iOS/Safari. Also: I did not like the idea of using JavaScript to fix issues that can also be manually fixed by adding the correct icons. That's something you'd have to do 1 time for you app using a tool like: https://app-manifest.firebaseapp.com/.

## Credits

- Sound files (squakk + nock + restart): https://freesound.org/people/yawfle/packs/367/
- Sound file HooYeah by LemonJolly: https://freesound.org/people/lemonjolly/sounds/273925/
- Icons: Refactoring UI
