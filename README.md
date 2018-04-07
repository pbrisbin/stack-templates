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
