### book-tracker-localization

This is the community language repository for [Book Tracker](https://apps.apple.com/us/app/book-tracker-bookshelf-log/id1491660771).

If there is a language you'd like to see Book Tracker localized to but we haven't got around to it yet, and you have some git-fu, feel free to submit a pull request to the repository.

Please do not add multiple languages in the same pull request — this way, there can be a discussion thread for each language for any changes or tweaks that need to be made, and give others opportunity for peer review.

### Disk Structure
Languages are structured in folders as such:

`en.lproj/xxx.strings`

Where `en` is replaced by the [ISO 639-1 two-letter language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes), and the `xxx.strings` files are structured as per the English (`en`) version.

All the files inside the folder must be translated. Please do not include any other files in a pull request.

### Localization

Strings are denoted as `"KEY"` = `"value"`, where the keys remain the same across all languages, and the values are localized. There must be a `;` at the end of each line.

`"SEARCH_PLACEHOLDER" = "Search";`

Where you see a `%@`, `%ld` or `{key}` token, this denotes a value that is replaced at runtime — in most cases will be the user-provided name for a space or tag, or a number. The corresponding localized value must keep the token in the right place to provide the same meaning as the English value.

`"FromToPages" = "From page %@ to page %@";`


### Credits

Please append the name you would like to be credited by to the pull request or the comment block at the top of the xxx.strings file.