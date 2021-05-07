# Democritus Uuids

[![PyPI](https://img.shields.io/pypi/v/d8s-uuids.svg)](https://pypi.python.org/pypi/d8s-uuids)
[![CI](https://github.com/democritus-project/d8s-uuids/workflows/CI/badge.svg)](https://github.com/democritus-project/d8s-uuids/actions)
[![Lint](https://github.com/democritus-project/d8s-uuids/workflows/Lint/badge.svg)](https://github.com/democritus-project/d8s-uuids/actions)
[![codecov](https://codecov.io/gh/democritus-project/d8s-uuids/branch/main/graph/badge.svg?token=V0WOIXRGMM)](https://codecov.io/gh/democritus-project/d8s-uuids)
[![The Democritus Project uses semver version 2.0.0](https://img.shields.io/badge/-semver%20v2.0.0-22bfda)](https://semver.org/spec/v2.0.0.html)
[![The Democritus Project uses black to format code](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://choosealicense.com/licenses/lgpl-3.0/)

Democritus functions<sup>[1]</sup> for working with uuids.

[1] Democritus functions are <i>simple, effective, modular, well-tested, and well-documented</i> Python functions.

We use `d8s` (pronounced "dee-eights") as an abbreviation for `democritus` (you can read more about this [here](https://github.com/democritus-project/roadmap#what-is-d8s)).

## Functions

  - ```python
    def uuid4_examples(n: int = 10, *, uuids_as_strings: bool = True) -> Union[List[str], List[uuid.UUID]]:
        """Create n uuids."""
    ```
  - ```python
    def uuid4() -> str:
        """Create a random UUID."""
    ```
  - ```python
    def uuid3(name: str, *, namespace: Optional[uuid.UUID] = None) -> str:
        """Create a random uuid based on the given name."""
    ```
  - ```python
    def uuid5(name: str, *, namespace: Optional[uuid.UUID] = None) -> str:
        """Create a random uuid based on the given name."""
    ```
  - ```python
    def is_uuid(possible_uuid: Union[str, uuid.UUID], *, version: Optional[int] = None) -> bool:
        """Return whether or not the possible_uuid is a uuid."""
    ```

## Development

👋 &nbsp;If you want to get involved in this project, we have some short, helpful guides below:

- [contribute to this project 🥇][contributing]
- [test it 🧪][local-dev]
- [lint it 🧹][local-dev]
- [explore it 🔭][local-dev]

If you have any questions or there is anything we did not cover, please raise an issue and we'll be happy to help.

## Credits

This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and Floyd Hightower's [Python project template](https://github.com/fhightower-templates/python-project-template).

[contributing]: https://github.com/democritus-project/.github/blob/main/CONTRIBUTING.md#contributing-a-pr-
[local-dev]: https://github.com/democritus-project/.github/blob/main/CONTRIBUTING.md#local-development-
