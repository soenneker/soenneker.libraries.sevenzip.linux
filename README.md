[![](https://img.shields.io/nuget/v/soenneker.libraries.sevenzip.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.sevenzip.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.sevenzip.linux/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.sevenzip.linux/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libraries.sevenzip.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.sevenzip.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.sevenzip.linux/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.sevenzip.linux/actions/workflows/codeql.yml)

# Soenneker.Libraries.SevenZip.Linux

The standalone 7-Zip command-line executable packaged for Linux .NET applications.

## Install

```bash
dotnet add package Soenneker.Libraries.SevenZip.Linux
```

The package copies `7zzs` beneath the application output directory:

```csharp
string sevenZip = Path.Combine(AppContext.BaseDirectory, "Resources", "7zzs");
```

Ensure `7zzs` is executable before starting it. Pass archive names, passwords, and output paths through `ProcessStartInfo.ArgumentList`; do not construct a shell command by concatenating them.

Always check the process exit code. When extracting untrusted archives, use a dedicated empty directory and enforce limits on archive size, extracted size, file count, and processing time before moving files into their final location.
