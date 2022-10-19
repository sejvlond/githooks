# Githooks

## Installation

Move all the files to you project into `.githooks` folder.

Setup git to use the folder for githooks
```
git config core.hooksPath .githooks
```

## Project specific configuration

Githooks supports configuration per project and per your dev flow.

Setup regex to search for ticket reference in branch name:
```
git config ticket-reference.rev-regex '^(JIRA-[0-9]+).*'
```

Setup regex to search for ticket reference in commit message:
```
git config ticket-reference.msg-regex '^(CRPT-[0-9]+).*'
```

## TODO
- [ ] document also insert strategy (prepend/append) and templates
- [ ] use the helpers in each script
- [ ] introduce `prepare-message` hook
- [ ] configurable logging/colors
