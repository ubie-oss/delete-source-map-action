# delete-source-map-action

A GitHub action for deleting [source map](https://developer.mozilla.org/en-US/docs/Tools/Debugger/How_to/Use_a_source_map) from web frontend distribution.

This action will do:

- Delete `*.map`
- Delete `sourceMappingURL=` comment in `*.js` and `*.css`

## Usage

An example for Next.js application:

```yml
- name: Delete source map
  uses: ubie-oss/delete-source-map-action@v1
  with:
    directory: ./.next/static
```
