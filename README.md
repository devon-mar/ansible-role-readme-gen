# readme_gen

This role generates a README for an Ansible role from role metadata. Role name, description and arguments
are taken from `galaxy_info.role_name`, `galaxy_info.description`, and `argument_specs.main.options` from
`meta/main.yml` respectively.

## Platforms
* GenericLinux

## Requirements
* None
## Notes
* The title of the README can be overridden by setting `title` in `meta/readme.yml`
* See `files/readme_argspec.yml` for possible keys for `readme.yml`.

## Role Variables
| Variable | Required | Type | Choices/Defaults | Comments |
|----------|----------|------|------------------|----------|
| `readme_gen_role_path` | True | str | | Path to the role |
| `readme_gen_dest` | False | str | `{{ readme_gen_role_path }}/README.md` | Destination file |
