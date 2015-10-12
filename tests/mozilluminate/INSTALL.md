How to install on production
============================
* Create an bot account on MozTrap
  * Write down the username and API key

* Copy this repo
* Change the `mtapi.mtorigin` in `tests/mozilluminate/sync.py:187`
* Change the default version number in `test/mozilluminate/moztrap_integration/moztrapcli/config.py`
* Remove the example file in `apps/example/test/manual/`
* Commit
* Push the code to a github repo
* Go to Travis CI, enable building the new github repo
* Set the environment variable `mz_user_name` and `mz_api_key`

* Add the example cases to `app/example/test/manual`, commit. (Make sure the diff contains only the added cases.)
* Check if the test passes on Travis, and check if the case is opend in MozTrap
