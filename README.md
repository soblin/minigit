# minigit

Learn the Rust programming language by implementing a very simple **git**.

## Milestone 

### Level1

Create a simple command line tool that works as follows.

```
$ cargo run init .
```

will create `.minigit/HEAD` file and write `.minigit/refs/main` in it.

```
$ cargo run add .
```

will create

- `.minigit/objects/sh/a-hash-of-that-file`
- `.minigit/index`

for those staged files.

```
$ cargo run commit -m "first commit"
```

will create

- tree object in `.minigit/objects/`
- commit object `.minigit/objects/`

and update `.minigit/refs/main`.
