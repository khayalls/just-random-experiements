# just-random-experiements

A scratchpad for small, self-contained experiments pulled from different projects: UI prototypes, interaction and motion tests, rendering tricks, design-to-code trials and quick proofs of concept.

Nothing here is a product. Each experiment is a throwaway or a starting point. It is kept so the idea and the code are easy to find again later.

## Projects

| Project | Parts |
| --- | --- |
| [QStore](qstore/) | [coupon-reward](qstore/coupon-reward/) |
| [Miscellaneous](misc/) | [xalca-naxisi](misc/xalca-naxisi/), [piksel-eller](misc/piksel-eller/), [kvadrat-dalga](misc/kvadrat-dalga/) |

## Layout

Experiments are grouped by the project they come from. Inside a project, each part gets its own folder:

```
just-random-experiements/
├── <project>/
│   ├── README.md          # what the project is, and a table of its parts
│   ├── <part>/
│   │   ├── README.md      # what it tries out, how to run it, design links
│   │   ├── index.html     # or whatever the experiment needs
│   │   └── assets/
│   └── <another-part>/
└── README.md              # this file
```

- Use lowercase kebab-case folder names: `qstore/coupon-reward`, not `QStore/CouponReward`.
- Name a part after the screen, component or idea it tries out.
- Use `misc/` for one-off experiments that don't belong to any project.

## Adding an experiment

1. Use the project's folder, or create one with a short `README.md` if it's a new project.
2. Create a folder for the part inside it.
3. Add a `README.md` to the part covering:
   - what it tries out
   - how to run it (for example `python3 -m http.server` in the folder, then open the printed URL)
   - links to related designs, references or a live preview
4. Keep the part's dependencies and assets inside its folder, so it runs without the rest of the repository.
5. Add a row to the project's table and to the **Projects** table above.

## Status

Experiments are added as they come up. Some will be polished and some won't, and any of them may be removed or rewritten.
