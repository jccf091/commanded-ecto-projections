# Changelog

## v0.7.1

### Bug fixes

- Ensure errors encountered while building the `Ecto.Multi` data structure within a `project` function are caught and passed to the `error/3` callback.

## v0.7.0

### Enhancements

- Support Commanded's event handler `error/3` callback ([#12](https://github.com/commanded/commanded-ecto-projections/pull/12)).

## v0.6.0

### Enhancements

- Pass through any additional projector configuration options to Commanded event handler.
  Allows new Commanded features to be used without updating this library (e.g. specify `consistency` option).

## v0.5.0

### Enhancements

- Allow an Ecto schema prefix to be defined in config or per handler ([#4](https://github.com/commanded/commanded-ecto-projections/pull/4)).


## v0.4.0

### Enhancements

- Add `repo` option to `Commanded.Projections.Ecto` macro ([#1](https://github.com/commanded/commanded-ecto-projections/pull/1)).
- Optional `after_update/3` callback function in projectors.
