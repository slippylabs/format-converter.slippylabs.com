# Data Format Converter

Convert between JSON, YAML, TOML, CSV and XML in any direction, with an explicit warning about anything the conversion cannot carry across. Runs entirely in your browser.

**Live:** <https://format-converter.slippylabs.com/>

## What it does

- JSON, YAML, TOML, CSV and XML, converted in any direction.
- Auto-detects the input format, or you can pin it.
- Send the output back to the input to chain conversions.
- Copy or download the result.

## How it works

Formats do not map onto each other cleanly, and the usual failure is that a converter drops what it cannot represent without telling you. This one keeps an explicit list of everything the conversion could not carry across — comments, type distinctions, attributes, ordering — and shows it alongside the output, so you find out before the data does.

## Run it locally

A static site. No build step, no package manager, no dependencies:

```
git clone git@github.com:slippylabs/format-converter.slippylabs.com.git
cd format-converter.slippylabs.com
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

---

Part of [Slippy Labs](https://slippylabs.com). Every tool is indexed at
[projects.slippylabs.com](https://projects.slippylabs.com).
