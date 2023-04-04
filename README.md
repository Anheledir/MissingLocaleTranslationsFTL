# Fluent FTL Translation Checker

This GitHub action checks your project's [Fluent FTL](https://projectfluent.org/) files for missing translations and creates GitHub issues for any discrepancies found. Fluent is a localization system by Mozilla, used to create multilingual applications with a simple and expressive syntax. FTL files are human-readable localization files that store translations for different languages.

## Usage

To use this action in your repository, follow these steps:

1. Create a new `.github/workflows/translation_check.yml` file in your repository.
2. Copy the contents of the provided `translation_check.yml` into the new file.
3. Update the `REFERENCE_FTL` environment variable in the `translation_check.yml` file to point to your reference FTL file, usually the one containing translations for your primary language.

This action will automatically run when a pull request is merged into the main branch, ensuring that your translations stay up-to-date and consistent.

## Why is it useful?

Keeping translations consistent across multiple languages can be challenging, especially when your project grows and evolves. This action helps to automate the process of identifying missing translations and creating issues for them, making it easier for contributors to identify what needs to be translated and keeping your project's localization up-to-date.

## Limitations

This action has a few limitations that you should be aware of when using it in your projects:

1. One FTL file per language: The action assumes that each language has a single FTL file containing all translations for that language. If your project uses multiple FTL files per language, the action may not work as expected, and you may need to modify the script to accommodate your project's structure.

2. Missing translations only: This action focuses on identifying missing translations and does not check for other issues, such as outdated translations, inconsistent terminology, or incorrect translations. Additional tools or manual review may be required to address these aspects of your localization process.

3. Limited to FTL files: This action is specifically designed for projects using Mozilla's Fluent localization system with FTL files. It is not suitable for other localization file formats, such as PO, JSON, or XLIFF.

4. GitHub issues: The action creates GitHub issues for missing translations, which might not be the preferred method for tracking translation tasks in every project. Depending on your project management practices, you may need to customize the action to integrate with other issue tracking systems or tools.

Despite these limitations, this action can still be a valuable tool for maintaining translation consistency across languages and streamlining the localization workflow in projects using Fluent FTL files.

## License

This action is released under the [MIT License](LICENSE). Feel free to use, modify, and distribute it as you see fit.

## Contributing

We welcome contributions from the community. If you have ideas for improvements or bug fixes, please create a pull request or open an issue in the repository.

## Reference Projects

- The Discord Bot "[Honeycomb](https://github.com/Anheledir/Honeycomb)"
- <*Your project could be here!*> 
