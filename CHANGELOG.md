# 1.3.1

* Enhancements
  * Fix cookbook issue when installing on `> Ubuntu 12.04`

# 1.3.0

* Enhancements
  * Added warning messages to startup when using github/file_store endpoints
  * Bump Octokit dependency to ~> 3.0

* Bug Fix
  * Fixed issue with GH indexing where there were a high number of repositories in an organization

# 1.2.2

* Enhancements
  * Bump to Reel 0.5
  * Set Celluloid log level to ERROR

* Bug Fixes
  * Include full URL to Github location in items cached by Github builder

# 1.2.0

* Enhancements
  * Loosen constraints and bump versions of various gems

* Bug Fixes
  * Fix issue with default configuration where home path was not being set

# 1.1.1

* Enhancements
  * Added /status endpoint to REST API

* Bug Fixes
  * Github cache builder will autopaginate to get all repos
  * Fix dependency issues with Faraday

# 1.1.0

* Enhancements
  * Added Github cache builder and Github endpoint. You can now add Github organization's as endpoints and the cache builder will crawl each repository looking for repositories which contain SemVer tags and raw cookbook metadata.

* Bug Fixes
  * Fix cache builder crashes when builder encounters a cookbook with invalid or missing metadata.
  * Invalid cookbooks won't be added to cache.

# 1.0.0

* Prioritize Cache Builders so their entries do not clobber one another
* An entire config file is checksumed so that when it changes, the cache is rebuilt
