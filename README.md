# airtap-demo

**Example of using [`airtap`](https://github.com/airtap/airtap) to unit test JavaScript in browsers.**

## Install

```
git clone git@github.com:airtap/demo.git && cd demo && npm i
```

## Usage

To test the browsers listed in [`.airtap.yml`](.airtap.yml):

```
npx airtap test.js
```

Test the default browser on your machine:

```
npx airtap --preset default test.js
```

Test with live reload (try modifying `test.js`):

```
npx airtap --live test.js
```

List available browsers:

```
npx airtap -la
```

Try adding [more providers and browsers](https://github.com/airtap/airtap#available-providers)! Or selecting more specific browsers, for example firefox that supports headless mode:

```yaml
browsers:
  - name: firefox
    supports:
      headless: true
```

## License

[MIT](LICENSE) © 2020-present Airtap contributors
