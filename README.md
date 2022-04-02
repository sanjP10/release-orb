# Release Orb
![CircleCI Build Status](https://circleci.com/gh/sanjP10/release-orb.svg?style=shield "CircleCI Build Status") [![CircleCI Orb Version](https://badges.circleci.com/orbs/sanjp10/release.svg)][reg-page] [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/sanjP10/release-orb/main/LICENSE)

This is an action that enables the use of the tool [release](https://github.com/sanjP10/release) in a CircleCI pipeline.
This exposes the use of the tool with a CircleCi interface.

## Usage

Example use as well as a list of available executors, commands, and jobs are available on this orb's [registry page][reg-page].

## Publishing Orb

Follow the official publishing orb [documents](https://circleci.com/docs/2.0/creating-orbs/#issue-a-new-release)

## Dev setup
To set up a dev orb to test with run the following.

```bash
circleci orb pack ./src | circleci orb publish - sanjp10/release@dev:alpha
```

## Updating Orb
Publish a semver version of the orb. relies on 
the commit subject containing the text `[semver:patch|minor|major|skip]`
as that will determine whether a patch, minor or major version will be published
or if publishing should be skipped.

## Resources

[CircleCI Orb Registry Page][reg-page] - The official registry page of this orb for all versions, executors, commands, and jobs described.

[reg-page]: https://circleci.com/orbs/registry/orb/sanjp10/release
