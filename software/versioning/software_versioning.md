# Versioning

When you create software you will need to mark its version. When you make changes to your software you need to increment the version somehow.

## Semantic Versioning (semVer)

A lot of software follows semantic versioning (semVer)  where versioning follows the Major.Minor.Patch (example: 1.3.2) format.

- Major: When the public-facing Application Programming Interface (API) changes in ways requiring client-side code changes
- Minor: When visible changes affect the client but require no changes on their part
- Patch: For bug fixes, small tweaks, and quality of life improvements

These versions use integers, which helps with effective sorting.

```text
["somePrefix-1.9.0", "somePrefix-1.10.0", "somePrefix-1.2.0"]
```

sorts as

```text
["somePrefix-1.10.0", "somePrefix-1.2.0", "somePrefix-1.9.0"]
```

when using string based sorting. When treated as 3 integers this isn't an issue.

## Calendar Versioning (calVer)

Some software uses calendar versioning. This sorts extremely well when done right.

```text
YYYY-MM-DD
```

This will sort naturaly well but there is one small risk that in a few thousand years... it won't. But then again, the Y2K issue did happen, at least this time ISO has us covered with

```text
+10000-01-01
```

for an extended format. Only systems hardcoded to expect 4 digitd only for the year will suffer. Personally, I'd just add a new era element to dates. 0-0000-00-01, the first day of the way off future era.

## Sequential / Incremental Versioning

This one is super simple. Each release you increment a counter. Some uses include

- Internal builds
- CI/CD artifacts
- Prototypes
- Firmware.

## TODO learn more
