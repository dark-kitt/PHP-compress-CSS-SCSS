# PHP compress CSS/SCSS

A small php script, to compress CSS/SCSS. Overwrites ids and classes with 'aa', 'ab', 'ac' etc..


## Note!

Matched only `getElementById`, `$(#id)`, `getElementsByClassName`, `addClass`, `hasClass`, `removeClass` and `$(.class)` in the JavaScript files.

## Usage

    require 'regex.php';
    require 'compressCSS.php';

    // if $selectors is null the function search for selectors with the given directory and file paths
    // or place the content in the array (e.g. ['cnt', 'cnt', etc.]) but don't mix content and directories
    $compressCSS = new compressCSS(
        $selectors,
        [$html],
        [$scss],
        [$js],
        $directory
    );
