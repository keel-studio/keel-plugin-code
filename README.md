# keel plugin: Code

The Code page: files, search, an editor and the changes on your branch. It is a host: Git, Code Review, Database and CI/CD add their tabs to it.

> **Status: planned.** The code still lives in [keel-v2](https://github.com/MiladNalbandi/keel-v2). It moves here step by step, as
> [the plugin plan](https://github.com/MiladNalbandi/keel-v2/tree/main/docs/plugins) says. There is nothing to install yet.

| | |
| --- | --- |
| id | `code` |
| needs | keel core (plugin SDK 1) |
| works with | — |
| parts | api · web |
| trust level | runs code in keel |

**What it adds to keel**

- the Code page (#/code)
- slots for its own plugins: `code.activity`, `code.tab`, `code.scm`

**Where the code is today (keel-v2)**

- `web/src/pages/Repo.tsx`
- `web/src/pages/repo/*`
- `keel.api.repo (the page's endpoints)` (api)

## Layout

```
keel-plugin.yml   the manifest
api/              Kotlin, a thin Spring Boot jar
web/              React pages and slots (an ES module)
```

## Install

When it is released: in keel, **Control › Plugins › Marketplace › Code › Install**. keel checks the file's
signature, shows what the plugin may do, and asks you before it installs.

## License

MIT
