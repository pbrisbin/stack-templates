> [!NOTE]
> All of my GitHub repositories have been **archived** and will be migrated to
> Codeberg as I next work on them. This repository either now lives, or will
> live, at:
>
> https://codeberg.org/pbrisbin/stack-templates
>
> If you need to report an Issue or raise a PR, and this migration hasn't
> happened yet, send an email to me@pbrisbin.com.

# Stack Templates

My personal stack templates.

## Usage

```
stack new [<option>, ...] <project> \
  https://raw.githubusercontent.com/pbrisbin/stack-templates/master/<name>.hsfiles
```

## Templates

### simple

Simple library-plus-executable.

- Hpack
- HSpec
- HLint, StylishHaskell, and Brittany configuration
- Circle-2.0 CI
- Makefile

See [Haskell Project Checklist](https://pbrisbin.com/posts/haskell_project_checklist/).

### yesod-docker

**NOTE**: This one is a bit out of date right now, and may not work.

- Yesod with [some updated conventions](https://pbrisbin.com/posts/tee-io_lessons_learned/)
- Docker-based development and Deployment

## Building Templates

Build any templates that are out of date with `sources/`:

```console
./shake
```

**NOTE**: shake won't know about new files, so use `--rebuild`.

Test templates by creating a project from them:

```console
./shake test
```
