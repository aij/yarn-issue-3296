This is an example of yarn prompting for which version of a package to install,
only to ignore the answer.


```
info Unable to find a suitable version for "history", please choose one by typing one of the numbers below:
  1) "history@^3.0.0" which resolved to "3.3.0"
  2) "history@ccap/history#3.3.0-ccap1" which resolved to "3.3.0"
Answer?:
```

Selecting 1 results in `yarn.lock.1`. Selecting 2 results in `yarn.lock.2`. Both are the same, and result in installing the version from NPM.

Running `npm update` instead does not prompt but installs the version from Github.