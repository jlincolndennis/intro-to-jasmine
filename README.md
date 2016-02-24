# Jasmine And Testing Stuff!

## Getting Set Up!

Install  jasmine:

```
npm install -g jasmine

```

Initialize jasmine in the folder where the testing magic is about to happen:

```
jasmine init
```

## Jasmine Naming Conventions

```
spec/leap_year_spec.js // Test
```

```
lib/leap_year_.js   // Thing We Are Testing
```

## Wiring Things Up

In spec folder, set up a variable referencing the code that will be tested:

```
var miles = require('../lib/miles')

```
Set up the test suite:

```
describe('Miles', function () {
  it('is our master plan here', function () {
    expect(somefunction()).toEqual('running stuff for realsies.')
  });
})
```

Set up a dummy function in order to check if things are wired correctly:

```
module.exports = {
  someFunction: function () {
    return 'running stuff for realsies.'
  }
}

```

This should yield a green result. (Run jasmine with $ jasmine) :
```
Started
.


1 spec, 0 failures
Finished in 0.007 seconds
```
