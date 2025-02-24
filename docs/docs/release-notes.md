
# Release Notes
=== "Python"

    ```py
    def main():
        print("Hello world!")

    if __name__ == "__main__":
        main()
    ```

=== "JavaScript"

    ```js
    function main() {
        console.log("Hello world!");
    }

    main();
    ```
=== "Python2"

    ```py title="add_numbers.py" linenums="1" hl_lines="2-4"
    # Fonksiyon deneme
    def add_two_numbers(num1, num2):
        return num1 + num2

    # Example usage
    result = add_two_numbers(5, 3)
    print('The sum is:', result)
    ```


---

## Upgrading

To upgrade MkDocs to the latest version, use pip:

```bash
pip install -U mkdocs
```

You can determine your currently installed version using `mkdocs --version`:

```console
$ mkdocs --version
mkdocs, version 1.5.0 from /path/to/mkdocs (Python 3.10)
```

## Development Team

The current and past members of the Row team.

* [@emsalsiz](https://github.com/emsals1z/)

## Version 1.6.1 (2024-08-30)

### Fixed

* Fix build error when environment variable `SOURCE_DATE_EPOCH=0` is set. #3795
* Fix build error when `mkdocs_theme.yml` config is empty. #3700
* Support `python -W` and `PYTHONWARNINGS` instead of overriding the configuration. #3809
* Support running with Docker under strict mode, by removing `0.0.0.0` dev server warning. #3784
* Drop unnecessary `changefreq` from `sitemap.xml`. #3629
* Fix JavaScript console error when closing menu dropdown. #3774
* Fix JavaScript console error that occur on repeated clicks. #3730
* Fix JavaScript console error that can occur on dropdown selections. #3694

### Added

* Added translations for Dutch. #3804
* Added and updated translations for Chinese (Simplified). #3684

## Version 1.6.0 (2024-04-20)

### Local preview

*   `mkdocs serve` no longer locks up the browser when more than 5 tabs are open. This is achieved by closing the polling connection whenever a tab becomes inactive. Background tabs will no longer auto-reload either - that will instead happen as soon the tab is opened again. Context: #3391

*   New flag `serve --open` to open the site in a browser.  
    After the first build is finished, this flag will cause the default OS Web browser to be opened at the home page of the local site.  
    Context: #3500

#### Drafts

> DANGER: **Changed from version 1.5.**
