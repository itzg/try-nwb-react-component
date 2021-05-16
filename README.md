This repo reproduces an issue with nwb v0.25.2 where the `nwb new` configuration running `npm run test` fails with

```
> npm run test

> try-nwb-react-component@1.0.0 test
> nwb test-react


START:
16 05 2021 10:01:49.363:INFO [karma-server]: Karma v5.0.9 server started at http://0.0.0.0:9876/
16 05 2021 10:01:49.366:INFO [launcher]: Launching browsers PhantomJS with concurrency unlimited
16 05 2021 10:01:49.437:INFO [launcher]: Starting browser PhantomJS
16 05 2021 10:01:59.800:INFO [PhantomJS 2.1.1 (Windows 8)]: Connected on socket k6ynVDimvC58zmVhAAAA with id 50452137
PhantomJS 2.1.1 (Windows 8) ERROR
  TypeError: Object is not a constructor (evaluating 'getPolyfill()')
  at webpack:///node_modules/reflect.getprototypeof/index.js:10:1 <- tests/index.test.js:35449:33

Finished in 0.459 secs / 0 secs @ 10:02:00 GMT-0500 (Central Daylight Time)

SUMMARY:
√ 0 tests completed
Karma exit code was 1
```