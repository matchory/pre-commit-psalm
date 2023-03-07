pre-commit-psalm
==================
A [pre-commit](https://pre-commit.com/) hook for [psalm](https://psalm.dev/).

This adds support for running [`vimeo/psalm`](https://psalm.dev) as a pre-commit hook in your PHP project.

Usage
-----

### Using Psalm with pre-commit
Add this to your `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/matchory/pre-commit-psalm
  rev: v1.0.0
  hooks:
    - id: psalm
```

Or, to enable automatic fixing with [Psalter](https://psalm.dev/docs/manipulating_code/fixing/):

```yaml
- repo: https://github.com/matchory/pre-commit-psalm
  rev: v1.0.0
  hooks:
    - id: psalm
      args: [ "--alter" ]
```

License
-------
MIT
