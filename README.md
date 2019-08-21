# prettier-eslint-dir-issue-repro

Reproducing <https://github.com/prettier/prettier-eslint-cli/issues/167>

## Install & Reproduce

```bash
npm it
```

## Output

```Terminal
> prettier-eslint-test@1.0.0 test /tmp/prettier-eslint-test
> prettier-eslint '**/*.js' --list-different

prettier-eslint-cli [ERROR]: There was an error formatting "level1-dir/level2-dir2/test.js":
    Error: EISDIR: illegal operation on a directory, read
level1-dir/level2-dir2/test.js/index.js
success formatting 1 file with prettier-eslint
failure formatting 1 file with prettier-eslint
1 file was unchanged
npm ERR! Test failed.  See above for more details.
```
