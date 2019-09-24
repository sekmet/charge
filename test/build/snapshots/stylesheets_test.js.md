# Snapshot report for `test/build/stylesheets_test.js`

The actual snapshot is saved in `stylesheets_test.js.snap`.

Generated by [AVA](https://ava.li).

## inlines stylesheets from npm packages

> Snapshot 1

    [
      'tmp/tests/target/index.css',
    ]

> Snapshot 2

    {
      'tmp/tests/target/index.css': `p {␊
        color: red;␊
      }␊
      ␊
      a {␊
        color: black;␊
      }`,
    }

## inlines stylesheets with relative @import statements to current directory

> Snapshot 1

    [
      'tmp/tests/target/index.css',
    ]

> Snapshot 2

    {
      'tmp/tests/target/index.css': `p {␊
        color: red;␊
      }␊
      ␊
      a {␊
        color: black;␊
      }`,
    }

## inlines stylesheets with relative @import statements to parent directory

> Snapshot 1

    [
      'tmp/tests/target/folder/index.css',
    ]

> Snapshot 2

    {
      'tmp/tests/target/folder/index.css': `p {␊
        color: red;␊
      }␊
      ␊
      a {␊
        color: black;␊
      }`,
    }

## transpiles stylesheets using Stage 2 features

> Snapshot 1

    [
      'tmp/tests/target/index.css',
    ]

> Snapshot 2

    {
      'tmp/tests/target/index.css': `body {␊
        font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, sans-serif;␊
      }`,
    }

## transpiles stylesheets using thee custom-media-queries feature from Stage 1

> Snapshot 1

    [
      'tmp/tests/target/index.css',
    ]

> Snapshot 2

    {
      'tmp/tests/target/index.css': `@media (max-width: 30em) {␊
        nav {␊
          display: none;␊
        }␊
      }`,
    }