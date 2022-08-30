# R2E2 Scenes

Some scenes are adapted from [Scenes for `pbrt-v3`](https://www.pbrt.org/scenes-v3) to work
with R2E2, including:

- **killeroo-tiny**: The classic "killeroo" model. Thanks to
  [headus](http://www.headus.com/au)/Rezard for the model.

- **bmw-m6**: BMW M6 car (model year 2006) illuminated by a realistic skylight
  model. Thanks to Fred C. M'ule Jr. ("tyrant monkey" on BlendSwap) for this
  nice car model. CC-Zero (public domain) license.


# Dumping the Scenes

1. Download and compile [R2E2's fork of `pbrt`](https://github.com/r2e2-project/pbrt-v3).

2. Run `pbrt --dumpscene <OUTPUT-DIR> [scene-name]/dump.pbrt`.

3. Remove extra files by running `./scripts/cleanup_dump.py <OUTPUT-DIR>`.

4. (Optional) Compress the dump by running `./scripts/compress_dump.py <SRC-DIR> <DST-DIR>`.

📝 **Note**: You can change the target treelet size by editing `maxtreeletbytes` property in `dump.pbrt`.
