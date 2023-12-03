# jscpd mirror

Mirror of jscpd package for pre-commit.

[pre-commit](https://github.com/pre-commit/pre-commit)

[jscpd](https://github.com/kucherenko/jscpd)

## Using eslint with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/maxpatiiuk/mirrors-jscpd
  rev: '' # Use the sha / tag you want to point at
  hooks:
    - id: jscpd
      # Optionally can add the following to restrict to certain file
      # types:
      # files \.[js]sx?$
      types: [text]
      # Optionally can specify additional arguments for the jscp
      # command:
      # args:
      #  --ignore "**/*.min.js,**/*.map,**/node_modules,**/tests"
      #  --reporters console
```
