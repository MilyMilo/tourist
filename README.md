# Tourist


### Note about testing:

Running the tests concurrently, with `yarn test` causes some false negatives. The CI workflow uses the `yarn test:ci`
command to run tests serially, which very rarely causes false negatives, but can be a hassle during development.

It is recommended to use `yarn test` for development, and just ignore the false negatives, or even only run tests 
selectively with `yarn ava -m "pattern"` - as described in the [ava docs](https://github.com/avajs/ava/blob/main/docs/05-command-line.md#running-tests-with-matching-titles)

With that said, there are some false negatives - if the tests fail, the best first step is just to run them again. 
If the failure is persistent then it might be a real problem.
