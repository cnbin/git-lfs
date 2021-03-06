# Git LFS Changelog

## v0.5.3 (23 July, 2015)

* `git lfs fetch` bugs #429 (@rubyist)
* Push can crash on 32 bit architectures #450 (@rubyist)
* Improved SSH support #404, #464 (@sinbad, @technoweenie)
* Support 307 redirects with relative url #442 (@sinbad)
* Fix `init` issues when upgrading #446 #451 #452 #465 (@technoweenie, @rubyist)
* Support chunked Transfer-Encoding #386 (@ryansimmen)
* Fix issue with pushing deleted objects #461 (@technoweenie)
* Teach `git lfs push` how to send specific objects #449 (@larsxschneider)
* Update error message when attempting to push objects that don't exist in `.git/lfs/objects` #447 (@technoweenie)
* Fix bug in HTTP client when response body is nil #472 #488 (@rubyist, @technoweenie)
* `-crlf` flag in gitattributes is deprecated #475 (@technoweenie)
* Improvements to the CentOS and Debian build and package scripts (@andyneff, @ssgelm)

## v0.5.2 (19 June, 2015)

* Add `git lfs fetch` command for downloading objects. #285 (@rubyist)
* Fix `git lfs track` issues when run outside of a git repository #312, #323 (@michael-k, @Aorjoa)
* Fix `git lfs track` for paths with spaces in them #327 (@technoweenie)
* Fix `git lfs track` by writing relative paths to .gitattributes #356 (@michael-k)
* Fix `git lfs untrack` so it doesn't remove entries incorrectly from .gitattributes #398 (@michael-k)
* Fix `git lfs clean` bug with zero length files #346 (@technoweenie)
* Add `git lfs fsck` #373 (@zeroshirts, @michael-k)
* The Git pre-push warns if Git LFS is not installed #339 (@rubyist)
* Fix Content-Type header sent by the HTTP client #329 (@joerg)
* Improve performance tracing while scanning refs #311 (@michael-k)
* Fix detection of LocalGitDir and LocalWorkingDir #312 #354 #361 (@michael-k)
* Fix inconsistent file mode bits for directories created by Git LFS #364 (@michael-k)
* Optimize shell execs #377, #382, #391 (@bozaro)
* Collect HTTP transfer stats #366, #400 (@rubyist)
* Support GIT_DIR and GIT_WORK_TREE #370 (@michael-k)
* Hide Git application window in Windows #381 (@bozaro)
* Add support for configured URLs containing credentials per RFC1738 #408 (@ewbankkit, @technoweenie)
* Add experimental support for batch API calls #285 (@rubyist)
* Improve linux build instructions for CentOS and Debian. #299 #309 #313 #332 (@jsh, @ssgelm, @andyneff)

## v0.5.1 (30 April, 2015)

* Fix Windows install.bat script.  #223 (@PeterDaveHello)
* Fix bug where `git lfs clean` will clean Git LFS pointers too #271 (@technoweenie)
* Better timeouts for the HTTP client #215 (@Mistobaan)
* Concurrent uploads through `git lfs push` #258 (@rubyist)
* Fix `git lfs smudge` behavior with zero-length file in `.git/lfs/objects` #267 (@technoweenie)
* Separate out pre-push hook behavior from `git lfs push` #263 (@technoweenie)
* Add diff/merge properties to .gitattributes #265 (@technoweenie)
* Respect `GIT_TERMINAL_PROMPT ` #257 (@technoweenie)
* Fix CLI progress bar output #185 (@technoweenie)
* Fail fast in `clean` and `smudge` commands when run without STDIN #264 (@technoweenie)
* Fix shell quoting in pre-push hook.  #235 (@mhagger)
* Fix progress bar output during file uploads.  #185 (@technoweenie)
* Change `remote.{name}.lfs_url` to `remote.{name}.lfsurl` #237 (@technoweenie)
* Swap `git config` order.  #245 (@technoweenie)
* New `git lfs pointer` command for generating and comparing pointers #246 (@technoweenie)
* Follow optional "href" property from git-lfs-authenticate SSH command #247 (@technoweenie)
* `.git/lfs/objects` spec clarifications: #212 (@rtyley), #244 (@technoweenie)
* man page updates: #228 (@mhagger)
* pointer spec clarifications: #246 (@technoweenie)
* Code comments for the untrack command: #225 (@thekafkaf)

## v0.5.0 (10 April, 2015)

* Initial public release
