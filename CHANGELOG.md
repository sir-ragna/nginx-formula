# Changelog

# CURRENT

- Add default log_format

# [2.4.0](https://github.com/saltstack-formulas/nginx-formula/compare/v2.3.3...v2.4.0) (2020-03-31)


### Bug Fixes

* **libtofs:** “files_switch” mess up the variable exported by “map.jinja” [skip ci] ([10b446e](https://github.com/saltstack-formulas/nginx-formula/commit/10b446ed1ed295e5bf75fcb437953df61b39ba9e))


### Continuous Integration

* **kitchen:** avoid using bootstrap for `master` instances [skip ci] ([efebb0a](https://github.com/saltstack-formulas/nginx-formula/commit/efebb0af6b4cda41a75d571fe5adc869b32febb7))


### Features

* **add purge option:** purge sites option ([a373bda](https://github.com/saltstack-formulas/nginx-formula/commit/a373bdab79e854c43c61de7edd65d460c73f0477))

## [2.3.3](https://github.com/saltstack-formulas/nginx-formula/compare/v2.3.2...v2.3.3) (2019-12-22)


### Bug Fixes

* **map.jinja:** use upstream default for `worker_connections` ([49caf8c](https://github.com/saltstack-formulas/nginx-formula/commit/49caf8cd69be49bd7773949c9f29e147732140a5)), closes [#261](https://github.com/saltstack-formulas/nginx-formula/issues/261)


### Continuous Integration

* **gemfile:** restrict `train` gem version until upstream fix [skip ci] ([09be54d](https://github.com/saltstack-formulas/nginx-formula/commit/09be54d05fb3ce7cff039aa74633a3b29dcbbcee))
* **travis:** quote pathspecs used with `git ls-files` [skip ci] ([091c614](https://github.com/saltstack-formulas/nginx-formula/commit/091c61448dd068e2734869caeb91cedb6f4264e2))
* **travis:** run `shellcheck` during lint job [skip ci] ([ccf64d9](https://github.com/saltstack-formulas/nginx-formula/commit/ccf64d9be2f0aa07dfb72ed25352197081e9e388))
* **travis:** use `major.minor` for `semantic-release` version [skip ci] ([facbaa1](https://github.com/saltstack-formulas/nginx-formula/commit/facbaa1e392de9238cf494964e57af73e1bf709a))

## [2.3.2](https://github.com/saltstack-formulas/nginx-formula/compare/v2.3.1...v2.3.2) (2019-11-25)


### Bug Fixes

* **certificates.sls:** prepare `certificates_path` dir separately ([297e3ac](https://github.com/saltstack-formulas/nginx-formula/commit/297e3ac400707cdd8f396da4c23ba30fc719a2cd)), closes [#241](https://github.com/saltstack-formulas/nginx-formula/issues/241)
* **release.config.js:** use full commit hash in commit link [skip ci] ([b13ec85](https://github.com/saltstack-formulas/nginx-formula/commit/b13ec85433d85b8ca87c3798db9cab3e297b81cf))


### Continuous Integration

* **kitchen:** use `debian-10-master-py3` instead of `develop` [skip ci] ([0665878](https://github.com/saltstack-formulas/nginx-formula/commit/066587829c5a40967b0e7926f12202b07b51ab3c))
* **kitchen:** use `develop` image until `master` is ready (`amazonlinux`) [skip ci] ([e8ed39a](https://github.com/saltstack-formulas/nginx-formula/commit/e8ed39a62cd40fe43af2aae67a3e2347d02b6b6a))
* **kitchen+travis:** upgrade matrix after `2019.2.2` release [skip ci] ([faefcab](https://github.com/saltstack-formulas/nginx-formula/commit/faefcabd654e5323b6ca146fb0046dd636ed5f68))
* **travis:** apply changes from build config validation [skip ci] ([4125887](https://github.com/saltstack-formulas/nginx-formula/commit/41258874a52df3da7a9f036b5378eb12b7a1a537))
* **travis:** opt-in to `dpl v2` to complete build config validation [skip ci] ([dbeb2da](https://github.com/saltstack-formulas/nginx-formula/commit/dbeb2da3e43aa13f162b1ac4c6203ecff60e0102))
* **travis:** update `salt-lint` config for `v0.0.10` [skip ci] ([a8382b5](https://github.com/saltstack-formulas/nginx-formula/commit/a8382b51a028ed5f069ff0168127ef3c8a4337da))
* **travis:** use build config validation (beta) [skip ci] ([bbf91c9](https://github.com/saltstack-formulas/nginx-formula/commit/bbf91c9f1432118a9eafde507de9ffa7b3ff5093))
* merge travis matrix, add `salt-lint` & `rubocop` to `lint` job ([567c08c](https://github.com/saltstack-formulas/nginx-formula/commit/567c08c9adf752eb95627b0e914804645015ee20))


### Documentation

* **contributing:** remove to use org-level file instead [skip ci] ([2e58d63](https://github.com/saltstack-formulas/nginx-formula/commit/2e58d636aaa8a66ec9540238b2f4e267172e10c2))
* **readme:** update link to `CONTRIBUTING` [skip ci] ([3ff6692](https://github.com/saltstack-formulas/nginx-formula/commit/3ff6692590932e7cc7609fdc0f52fc261228f290))


### Performance Improvements

* **travis:** improve `salt-lint` invocation [skip ci] ([e586fbe](https://github.com/saltstack-formulas/nginx-formula/commit/e586fbeebc758cdfd6d381a6ef9ad72231523dea))


### Tests

* **pillar/nginx.sls:** add reprodicible snippet based on issue [#241](https://github.com/saltstack-formulas/nginx-formula/issues/241) ([4ba3524](https://github.com/saltstack-formulas/nginx-formula/commit/4ba35247ed742393367968db34ff61a6b07f6695))

## [2.3.1](https://github.com/saltstack-formulas/nginx-formula/compare/v2.3.0...v2.3.1) (2019-10-10)


### Bug Fixes

* **certificates.sls:** fix `salt-lint` errors ([](https://github.com/saltstack-formulas/nginx-formula/commit/bedc1b6))
* **map.jinja:** fix `salt-lint` errors ([](https://github.com/saltstack-formulas/nginx-formula/commit/0772d8a))
* **pkg.sls:** fix `salt-lint` errors ([](https://github.com/saltstack-formulas/nginx-formula/commit/06d055e))


### Continuous Integration

* **kitchen:** change `log_level` to `debug` instead of `info` ([](https://github.com/saltstack-formulas/nginx-formula/commit/671a4ce))
* **kitchen:** install required packages to bootstrapped `opensuse` [skip ci] ([](https://github.com/saltstack-formulas/nginx-formula/commit/17291a0))
* **kitchen:** use bootstrapped `opensuse` images until `2019.2.2` [skip ci] ([](https://github.com/saltstack-formulas/nginx-formula/commit/a39e124))
* **platform:** add `arch-base-latest` ([](https://github.com/saltstack-formulas/nginx-formula/commit/c921086))
* **yamllint:** add rule `empty-values` & use new `yaml-files` setting ([](https://github.com/saltstack-formulas/nginx-formula/commit/3d48b1b))
* merge travis matrix, add `salt-lint` & `rubocop` to `lint` job ([](https://github.com/saltstack-formulas/nginx-formula/commit/08ce3ed))
* use `dist: bionic` & apply `opensuse-leap-15` SCP error workaround ([](https://github.com/saltstack-formulas/nginx-formula/commit/8ddb921))


### Documentation

* **pillar.example:** fix TOFS comment to explain the default path [skip ci] ([](https://github.com/saltstack-formulas/nginx-formula/commit/714f547)), closes [/github.com/saltstack-formulas/libvirt-formula/pull/60#issuecomment-537965254](https://github.com//github.com/saltstack-formulas/libvirt-formula/pull/60/issues/issuecomment-537965254) [/github.com/saltstack-formulas/libvirt-formula/pull/60#issuecomment-537988138](https://github.com//github.com/saltstack-formulas/libvirt-formula/pull/60/issues/issuecomment-537988138)

# [2.3.0](https://github.com/saltstack-formulas/nginx-formula/compare/v2.2.1...v2.3.0) (2019-09-01)


### Continuous Integration

* **kitchen+travis:** replace EOL pre-salted images ([70e1426](https://github.com/saltstack-formulas/nginx-formula/commit/70e1426))


### Features

* **passenger:** inc config, snippets, servers, etc ([e07b558](https://github.com/saltstack-formulas/nginx-formula/commit/e07b558))

## [2.2.1](https://github.com/saltstack-formulas/nginx-formula/compare/v2.2.0...v2.2.1) (2019-08-25)


### Documentation

* **readme:** update testing section ([182f216](https://github.com/saltstack-formulas/nginx-formula/commit/182f216))

# [2.2.0](https://github.com/saltstack-formulas/nginx-formula/compare/v2.1.0...v2.2.0) (2019-08-12)


### Features

* **yamllint:** include for this repo and apply rules throughout ([6b7d1fe](https://github.com/saltstack-formulas/nginx-formula/commit/6b7d1fe))

# [2.1.0](https://github.com/saltstack-formulas/nginx-formula/compare/v2.0.0...v2.1.0) (2019-08-04)


### Continuous Integration

* **kitchen+travis:** modify matrix to include `develop` platform ([f6b357d](https://github.com/saltstack-formulas/nginx-formula/commit/f6b357d))


### Features

* **linux:** archlinux support (no osfinger grain) ([ab6148c](https://github.com/saltstack-formulas/nginx-formula/commit/ab6148c))

# [2.0.0](https://github.com/saltstack-formulas/nginx-formula/compare/v1.1.0...v2.0.0) (2019-06-19)


### Bug Fixes

* **snippets:** removed appending of ".conf" ([aa87721](https://github.com/saltstack-formulas/nginx-formula/commit/aa87721))


### BREAKING CHANGES

* **snippets:** Users have to modify their pillar
according to this commit. Users MUST append '.conf' for their
existing managed snippets.

# [1.1.0](https://github.com/saltstack-formulas/nginx-formula/compare/v1.0.5...v1.1.0) (2019-06-03)


### Features

* **tofs:** first implemetation + tplroot ([d5262ea](https://github.com/saltstack-formulas/nginx-formula/commit/d5262ea))

## [1.0.5](https://github.com/saltstack-formulas/nginx-formula/compare/v1.0.4...v1.0.5) (2019-05-13)


### Documentation

* **readme:** improve readme sections ([3cc3407](https://github.com/saltstack-formulas/nginx-formula/commit/3cc3407))

## [1.0.4](https://github.com/saltstack-formulas/nginx-formula/compare/v1.0.3...v1.0.4) (2019-05-13)


### Bug Fixes

* prevent running of states deprecated in `v1.0.0` ([46dff15](https://github.com/saltstack-formulas/nginx-formula/commit/46dff15))

## [1.0.3](https://github.com/saltstack-formulas/nginx-formula/compare/v1.0.2...v1.0.3) (2019-05-13)


### Documentation

* **readme:** add warning banner about `v1.0.0` breaking changes ([d553821](https://github.com/saltstack-formulas/nginx-formula/commit/d553821))

## [1.0.2](https://github.com/saltstack-formulas/nginx-formula/compare/v1.0.1...v1.0.2) (2019-05-12)


### Documentation

* **readme:** update README, add badges ([adbac43](https://github.com/saltstack-formulas/nginx-formula/commit/adbac43))

## [1.0.1](https://github.com/saltstack-formulas/nginx-formula/compare/v1.0.0...v1.0.1) (2019-05-12)


### Documentation

* remove obsolete CHANGELOG.rst file ([698aadb](https://github.com/saltstack-formulas/nginx-formula/commit/698aadb))

# [1.0.0](https://github.com/saltstack-formulas/nginx-formula/compare/v0.56.1...v1.0.0) (2019-05-12)


### Build System

* remove obsolete Makefile ([4961b04](https://github.com/saltstack-formulas/nginx-formula/commit/4961b04))


### Code Refactoring

* replace old `nginx` with `nginx.ng` ([0fc5070](https://github.com/saltstack-formulas/nginx-formula/commit/0fc5070))


### BREAKING CHANGES

* all previous `nginx` based configurations must be reviewed;
`nginx.ng` usage must be promoted to `nginx` and any uses of the original
`nginx` will have to be converted.

## [0.56.1](https://github.com/saltstack-formulas/nginx-formula/compare/v0.56.0...v0.56.1) (2019-04-27)


### Tests

* **inspec:** add test for `log_format` [#219](https://github.com/saltstack-formulas/nginx-formula/issues/219) ([4ed788e](https://github.com/saltstack-formulas/nginx-formula/commit/4ed788e))

# [0.56.0](https://github.com/saltstack-formulas/nginx-formula/compare/v0.55.1...v0.56.0) (2019-04-26)


### Features

* **`pillar.example`:** add stock `log_format` ([95ff308](https://github.com/saltstack-formulas/nginx-formula/commit/95ff308))

## [0.55.1](https://github.com/saltstack-formulas/nginx-formula/compare/v0.55.0...v0.55.1) (2019-04-26)


### Documentation

* **semantic-release:** implement an automated changelog ([569b07a](https://github.com/saltstack-formulas/nginx-formula/commit/569b07a))
