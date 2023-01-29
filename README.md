# DisTube Example

DisTube.js.org example music bot with command handler

**Dependencies maybe outdated. You should update them yourself!**

Check out the [official guide](https://distube.js.org/guide) to get your music bot running from scratch.

**Useful commands for CI/CD**

prerequisites:

* Install `jq` and `moreutils`(use of sponge)

Commands:

* Replaces an existing value (test) from `test.json` file, this is useful to replace token var before deployment

  ```Bash
  export export_var=value
  jq --arg exportVar "$export_var" '.test = $exportVar' test.json|sponge test.json
  ```
