# master

* Speed up `hashStrings` by using `MD5` (instead of `SHA256`).

# 0.2.2

* Make `hashTree` match after `copyRecursivelySync`, by disregarding the
  name of the root directory and not including directory times

# 0.2.1

* Make readdir ordering deterministic

# 0.2.0

* Remove `linkRecursivelySync` & `linkAndOverwrite`

# 0.1.2

* Add `copyRecursivelySync` & `copyPreserveSync`
* Change `linkRecursivelySync` & `linkAndOverwrite` to use
  `copyRecursivelySync` & `copyPreserveTime` respectively. We now refuse
  to overwrite in either of those functions, despite the `linkAndOverwrite`
  name.

# 0.1.1

* In `linkRecursivelySync`, link (broken) symlinks correctly

# 0.1.0

* Initial release
