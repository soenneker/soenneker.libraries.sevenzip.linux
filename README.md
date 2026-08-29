[![](https://img.shields.io/nuget/v/soenneker.libraries.sevenzip.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.sevenzip.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.sevenzip.linux/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.sevenzip.linux/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libraries.sevenzip.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.sevenzip.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.sevenzip.linux/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.sevenzip.linux/actions/workflows/codeql.yml)

# Soenneker.Libraries.SevenZip.Linux

Adds the 7zip Linux executable, updated daily (if available).

## Install

```bash
dotnet add package Soenneker.Libraries.SevenZip.Linux
```

## What it provides

- Adds the 7zip Linux executable, updated daily (if available).
- The file is copied to the output directory, and located at the relative path: `Resources\`.

## How to use it

After installation, resolve the packaged file from the output-relative path above. The package deploys the asset but does not invoke it for you.
