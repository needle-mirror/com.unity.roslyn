# Changelog

All notable changes to this package will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [0.2.2-preview] - 2022-04-04
- Disable loading ExternalCompiler when package is installed with Unity 2021 and later.

## [0.2.1-preview] - 2022-01-21
- Updates to package for next Entities release.

## [0.2.0-preview] - 2022-01-21
- Updates to package for next Entities release.

## [0.1.3-preview] - 2021-10-05
- No longer ignore CS0282 warnings (now handled by DiagnosticSuppressor) and don't report info as warnings (no longer report info).

## [0.1.2-preview] - 2020-05-17
- Ignore CS0649 warning (needed to augment valuetypes with partial).

## [0.1.1-preview] - 2020-02-02
- Ignore CS0649 and CS0169 warnings when PlayerSettings.suppressCommonWarnings is enabled.
- Bump minimum version to 2020.2.

## [0.0.4-preview] - 2020-01-28
- Ensure that `RunOnlyOnAssembliesWithReference` also runs on the assembly that is being referenced (required for Unity.Entities).
- Fix ExternalCSharpCompiler to correctly run Linux version of the compiler on Linux platforms.

## [0.0.3-preview] - 2020-12-02
- Update license, documentation and third party notice for release

## [0.0.2-preview] - 2020-11-23
- Fix issue with output path containing space.

## [0.0.1-preview] - 2020-11-18
- Fail gracefully on package upgrade

## [0.0.0-preview.10] - 2020-10-27
- Update roslyn version.
- Remove workaround for not requiring partial classes for additional source generation.

## [0.0.0-pre.9] - 2020-09-29
- Fix semver package version and update package description.
- Update documentation.

## [0.0.0-preview.8] - 2020-09-29
- Fix to use full path when adding generators to command-line options.

## [0.0.0-preview.7] - 2020-09-24
- Fix minor issue issue with debugging by default.

## [0.0.0-preview.6] - 2020-09-23
- Optimizations to discovery of source generators.
- Remove discovery of source generators in SourceGenerator~ folder (must now be labeled with asset labels below).

## [0.0.0-preview.5] - 2020-09-19

### Changed
- Discover generator plugins in assets if they have the `SourceGenerator` asset label.
- Ignore running generators even if they have the `SourceGenerator` label, if they also have the `RunOnlyOnAssembliesWithReference` label and don't reference the assembly in which the generator lives (to selectively target generators).
- Pass in current working directory as first additional file if using generators.
- Optimize by running csc in `/shared` mode (run with shared compiler server process).
- Lots more logging/profiling.

## [0.0.0-preview.4] - 2020-09-15

### Changed
- Ensure that the ExternalCSharpCompiler assembly is visible to Unity.Entities.CodeGen.Tests (instead of Unity.Entities.Hybrid.CodeGen.Tests).

## [0.0.0-preview.3] - 2020-08-31

### Added
- Added a helper method called GetReferencedSystemDllFullPaths() to the ExternalCompiler class to retrieve required .NET Standard 2.0 system references when running integration tests.

### Changed
- Ensured that the ExternalCSharpCompiler assembly is visible to Unity.Entities.Hybrid.CodeGen.Tests.

## [0.0.0-preview.2] - 2020-07-24

### Added
- Test

### Changed
- Test

### Fixed
- Test

## [0.1.0] - 2020-06-24

### This is the first release of *Unity Package Roslyn*.

Add trivia about Roslyn here