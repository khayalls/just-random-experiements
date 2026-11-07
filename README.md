# just-random-experiements

A scratchpad for small, self-contained experiments pulled from different projects: UI prototypes, interaction and motion tests, rendering tricks, design-to-code trials and quick proofs of concept.

Nothing here is a product. Each experiment is a throwaway or a starting point. It is kept so the idea and the code are easy to find again later.

## Layout

Each experiment gets its own folder at the root of the repository and does not depend on the others:

```
just-random-experiements/
├── <experiment-name>/
│   ├── README.md      # what it is, where it came from, how to run it
│   └── ...            # the experiment's own files and assets
└── README.md
```

Name folders in lowercase kebab-case after the idea, with the source project as a prefix if it helps (for example `qstore-coupon-reward`).

## Adding an experiment

1. Create a new folder for it.
2. Add a short `README.md` covering:
   - what the experiment tries out
   - which project it came from, if any
   - how to run it (for example `python3 -m http.server` in the folder, then open the printed URL)
   - links to related designs or references
3. Keep its dependencies inside the folder, so it runs without the rest of the repository.

## Status

Experiments are added as they come up. Some will be polished and some won't, and any of them may be removed or rewritten.
