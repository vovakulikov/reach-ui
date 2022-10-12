# @reach/checkbox

## 0.18.0-pre.3

### Patch Changes

- Updated dependencies:
  - `@reach/auto-id@0.18.0-pre.3`
  - `@reach/machine@0.18.0-pre.3`
  - `@reach/utils@0.18.0-pre.3`

## 0.18.0-pre.2

### Patch Changes

- Updated dependencies:
  - `@reach/auto-id@0.18.0-pre.2`
  - `@reach/machine@0.18.0-pre.2`
  - `@reach/utils@0.18.0-pre.2`

## 0.18.0-pre.1

### Minor Changes

- The output directory structure has changed slightly. Module files are now named `reach-<pkg>.mjs` instead of `reach-<pkg>.esm.js`. ([`6e40773f`](https://github.com/reach/reach-ui/commit/6e40773fc0f430dba9029fee57b526a7eb25827e))

### Patch Changes

- Updated dependencies:
  - `@reach/auto-id@0.18.0-pre.1`
  - `@reach/machine@0.18.0-pre.1`
  - `@reach/utils@0.18.0-pre.1`

## 0.18.0-pre.0

### Minor Changes

- We have simplified our build setup to remove a boatload of dependencies. Build output for all packages may look slightly different, though functionally packages that don't have explicit changes marked in the release notes have not changed. ([`c2a1794b`](https://github.com/reach/reach-ui/commit/c2a1794b6818822080f428a1cbe2cec2b4a0a218))

  This may affect you if you use `patch-package` to modify output code. If you need support for legacy browsers, the new bundle may not transpile the same ECMA features as before. In that case you may want to transpile Reach packages directly.

- Uncontrolled input fields inside of a form will now be reset to their default values or cleared on `form.reset` ([`79319a75`](https://github.com/reach/reach-ui/commit/79319a75a639db398c62ca3296896894eb3e539e))
- All default exports have been removed. Replace all default imports with the appropriate documented named export. ([`79319a75`](https://github.com/reach/reach-ui/commit/79319a75a639db398c62ca3296896894eb3e539e))

### Patch Changes

- `useMixedCheckbox` mistakenly derived its `checked` value incorrectly. In practice this was unlikely to cause an issue, but it now derives the guaranteed value from the active component state. ([`79319a75`](https://github.com/reach/reach-ui/commit/79319a75a639db398c62ca3296896894eb3e539e))
- Updated dependencies:
  - `@reach/auto-id@0.18.0-pre.0`
  - `@reach/machine@0.18.0-pre.0`
  - `@reach/utils@0.18.0-pre.0`