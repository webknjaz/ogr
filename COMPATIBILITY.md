# Compatibility table for services

Methods/properties not listed in here are implemented for all services.
In case you find any error, please [create a new issue](https://github.com/packit/ogr/issues/new).

## Comments

### `IssueComment`

|                  | GitHub | GitLab | Pagure |
| ---------------- | :----: | :----: | :----: |
| `body` (get/set) |  ✔/✔   |  ✔/✔   |  ✔/✘   |
| `add_reaction`   |   ✔    |   ✔    |   ✘    |
| `get_reactions`  |   ✔    |   ✔    |   ✘    |

### `PRComment`

|                  | GitHub | GitLab | Pagure |
| ---------------- | :----: | :----: | :----: |
| `body` (get/set) |  ✔/✔   |  ✔/✔   |  ✔/✘   |
| `add_reaction`   |   ✔    |   ✔    |   ✘    |
| `get_reactions`  |   ✔    |   ✔    |   ✘    |
| `closed_by`      |   ✘    |   ✘    |   ✔    |

## Issue

|             | GitHub | GitLab | Pagure |
| ----------- | :----: | :----: | :----: |
| `add_label` |   ✔    |   ✔    |   ✘    |

## Pull request

|                   | GitHub | GitLab | Pagure |
| ----------------- | :----: | :----: | :----: |
| `add_label`       |   ✔    |   ✔    |   ✘    |
| `get_all_commits` |   ✔    |   ✔    |   ✘    |
| `labels`          |   ✔    |   ✔    |   ✘    |

## Release

|                   | GitHub | GitLab |          Pagure          |
| ----------------- | :----: | :----: | :----------------------: |
| `edit_release`    |   ✔    |   ✘    |            ✘             |
| `body` (only get) |   ✔    |   ✔    | ✘ (returns empty string) |

## Commit flag

|          | GitHub | GitLab | Pagure |
| -------- | :----: | :----: | :----: |
| `edited` |   ✔    |   ✘    |   ✔    |

## Project

|                      | GitHub | GitLab |         Pagure          |
| -------------------- | :----: | :----: | :---------------------: |
| `change_token`       |   ✘    |   ✔    |            ✔            |
| `get_release`        |   ✔    |   ✔    |            ✘            |
| `get_latest_release` |   ✔    |   ✔    |            ✘            |
| `is_private`         |   ✔    |   ✔    | ✘ (may not be accurate) |

## User

|                | GitHub | GitLab | Pagure |
| -------------- | :----: | :----: | :----: |
| `get_projects` |   ✔    |   ✘    |   ✔    |
| `get_forks`    |   ✔    |   ✘    |   ✔    |
| `get_email`    |   ✔    |   ✔    |   ✘    |

## Reaction

|          | GitHub | GitLab | Pagure |
| -------- | :----: | :----: | :----: |
| `delete` |   ✔    |   ✔    |   ✘    |
