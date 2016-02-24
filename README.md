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

## Making The Test

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
