# Solid Lints
[![style: solid](https://img.shields.io/badge/style-solid-orange)](https://pub.dev/packages/solid_lints)
[![$solid_lints](https://nokycucwgzweensacwfy.supabase.co/functions/v1/get_project_badge?projectName=solid_lints)](https://www.worklog.ai)


Flutter/Dart lints configuration based on software engineering industry standards (ISO/IEC, NIST) and best practices.

# Usage

Add dependency in your pubspec.yaml:

```yaml
dev_dependencies:
  solid_lints: <INSERT LATEST VERSION>
```

And then include `solid_lints` into your project top-level `analysis_options.yaml`:

```yaml
include: package:solid_lints/analysis_options.yaml
```

Also you can use a specialized rule set designed for Dart tests.
Add an `analysis_options.yaml` file under the `test/` directory, and include the ruleset:

```yaml
include: package:solid_lints/analysis_options_test.yaml
```

Then you can see suggestions in your IDE or you can run checks manually:

```bash
dart analyze;
dart run dart_code_metrics:metrics analyze lib test;
dart run dart_code_metrics:metrics check-unused-files lib test;
dart run dart_code_metrics:metrics check-unused-l10n lib test;

```
Beware that some of the `dart_code_metrics` checks are not displayed in IDE so running checks 
manually or in your actions (CI) is essential.

Learn more: https://github.com/dart-code-checker/dart-code-metrics#cli
# Badge

To indicate that your project is using Solid Lints, you can use the following badge:

```markdown
[![style: solid](https://img.shields.io/badge/style-solid-orange)](https://pub.dev/packages/solid_lints)
```
