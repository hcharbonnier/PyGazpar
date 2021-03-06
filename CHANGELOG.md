# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.14] - 2020-09-23
### Fixed
- GrDF survey popup has to be closed at the home page.
- GrDF Assistant popup may hide the Download button. We have to close it.
- GrDF bottom banner that invite to accept cookies may also hide the Download button. We have to accept it.

### Added
- A new parameter 'lastNRows' to get only the last N most recent records.

## [0.1.13] - 2020-06-30
### Fixed
- GrDF data retrieval from Excel file is not limited to the 1000 first rows any more.

## [0.1.12] - 2020-06-30
### Fixed
- The previous 0.1.11 is not sufficient. Hence, 2 new changes : First, make configurable the waiting time so the user can adapt to its context usage.
Second, the condition on clicking on Download button is now based on the corresponding event and not anymore on its identifier. 

## [0.1.11] - 2020-06-29
### Fixed
- When GrDF Web site is slower than usual, the client may not wait enough time for pages to load and miss to reach the data file.
It occurs with the page containing 'Jour' button which is very long to load (I increase the wait to load time from 5s to 30s).

## [0.1.10] - 2020-06-03
### Fixed
- Extract rows from Excel until line 1000 (instead of 365 as before).

## [0.1.9] - 2019-08-31
### Fixed
- WebDriver window size must be large enough to display all clickable components.

## [0.1.8] - 2019-08-31
### Changed
- Use PropertyNameEnum type to store all property names.

## [0.1.7] - 2019-08-29
### Added
- Add wait_time option to control how much time the library has to wait for Web page element to load (see https://selenium-python.readthedocs.io/waits.html for details).
- Add LoginError exception raised when PyGazpar is unable to sign in the GrDF Web site with the given username/password.
- Refactor all data property names.

## [0.1.6] - 2019-08-26
### Added
- Add README.md and CHANGELOG.md.
- Add Client.data() method to get the updated data.

### Removed
- Remove Client.data property to get the updated data. Replaced with Client.__data private property.

[Unreleased]: https://github.com/ssenart/PyGazpar/compare/0.1.9...HEAD
[0.1.13]: https://github.com/ssenart/PyGazpar/compare/0.1.12...0.1.13
[0.1.12]: https://github.com/ssenart/PyGazpar/compare/0.1.11...0.1.12
[0.1.11]: https://github.com/ssenart/PyGazpar/compare/0.1.10...0.1.11
[0.1.10]: https://github.com/ssenart/PyGazpar/compare/0.1.9...0.1.10
[0.1.9]: https://github.com/ssenart/PyGazpar/compare/0.1.7...0.1.9
[0.1.8]: https://github.com/ssenart/PyGazpar/compare/0.1.7...0.1.8
[0.1.7]: https://github.com/ssenart/PyGazpar/compare/0.1.6...0.1.7
[0.1.6]: https://github.com/ssenart/PyGazpar/compare/0.1.5...0.1.6
