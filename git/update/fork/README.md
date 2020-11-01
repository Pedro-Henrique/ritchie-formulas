<!-- markdownlint-disable-file MD013 -->

# Git update fork

## Premisses

- git installed
- being run in UNIX environment

## Command

- Prompt

```bash
rit git update fork
```

- Docker

```bash
rit git update fork --docker
```

- Stdin

<!-- Select destination branch (default: master): asdf
? Set upstream ? (only first time) false
? Push after update ? false -->


```bash
echo '{"branch": "my_brach", "setupstream": true, "push": true}' | rit git update fork --stdin
```

- Stdin + Docker

```bash
echo '{"branch": "my_brach", "setupstream": true, "push": true}' | rit git update fork --stdin --docker
```

## Description

Update a fork on github.

It allows the user to inform 3 different kinds of inputs:

- destination branch (text)

- upstream (boolean)

- Push after update (boolean)

## Demo

![Alt Text](https://media.giphy.com/media/VdQGuZoyozL9J1Lhhl/giphy.gif)