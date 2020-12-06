# Utgs

A library that can be used by the Google AppsScript's online editor to conduct unit tests. Stands for Unit Testing with Google appsScripts.

Documentation on usage available in /docs.

## Quickstart

The project id is `1cSXAtmjHA61q0KXQLo4nVq7M2ISdhIq01qucWxbpPqZGYldoxE-hxF2R`. The default identifier is `Utgs`

```js
function Tests () {
  // sorta like importing, this inits the variables
  const {describe, it, asset} = Utgs.module(); 

  // conduct your tests
  describe("Test Category 1", function () {
    it("This one fails", function () {
      assert.equals({
        comment: 'If it fails, it displays in the log',
        expected: 'Yes',
        actual: 'No'
      });
    });
  });
}
```

Can also be installed via node, `npm install @classroomtechtools/unittesting`.

## Unit tests!

This package has unit tests on itself, which is also useful to check out how to use it.

`npm run test`

## Motivation

Unit testing is worth it.

## Thanks

Much of the original code came from [GSUnit](https://sites.google.com/site/scriptsexamples/custom-methods/gsunit), with additional refactoring and the additional function assertions.

