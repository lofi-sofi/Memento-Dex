# Memento Dex

**A short game about the things you remember, and the things you don't.** 

A creature collector game about memory — how we keep it, how we lose it, and
different ways you can meet someone whose reality might be different than yours.

🔗 **[Read the site →](https://lofi-sofi.github.io/Memento-Dex/)**

---

## What's in this repo

This is the landing page and public dev log for the game — not the game itself.

| File | What it is |
| --- | --- |
| `index.html` | The whole site. HTML, CSS and JS in one file. No build step, no dependencies. |

---

## About the game

If you were a kid with a handheld, you know the ritual: meet a creature, catch a
creature, watch the entry appear in your index. Memento Dex is built on that muscle
memory on purpose — the format is doing work here, not decoration.

It's a game about cognitive decline, and the angle matters: nobody in it is a monster,
and forgetting is not the horror. The goal is that you come out the other side with a
little more patience, not a little more fear.

**Status:** in development. Story and art in progress, prototype playable, no date yet.

---

## Editing the site

Everything you'd want to change lives in the `CONFIG` block near the bottom of
`index.html`. Nothing else needs touching.

### Wiring up the email form

The signup form posts to [Formspree](https://formspree.io). Create a form there, then
paste the endpoint into the constant:

```js
const FORMSPREE_ENDPOINT = "https://formspree.io/f/yourformid";
```

Left empty, the form stays functional — it just points people at the contact email
instead of failing silently.

### Adding a dev log entry

Copy a block, put it at the **top** of the `DEV_LOG` array. Newest first.
`body` takes one string or several; each becomes its own paragraph.

```js
const DEV_LOG = [
  {
    date: "2026-08-05",
    title: "Naming things, and a coincidence I'm keeping",
    body: [
      "First paragraph.",
      "Second paragraph."
    ]
  },
  // older entries below
];
```

---

## Deploying

Served with GitHub Pages from the root of `main`. Push to `main` and the live site
updates within a minute or two.

---

## Contact

Questions, or want to be told when there's something to play —
**lofisophidev@gmail.com**

---

*Built with heart first.*
