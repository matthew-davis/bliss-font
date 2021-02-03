# bliss-font
An icon font containing the characters, diacritics and words defined by Blissymbolics Communication International.

### Folder Structure
* css - Stylesheets for WebFonts
* json - JSON maps for the symbols
* svgs - indvidual svg files for each of the symbols
* ts - TypeScript decleration file for the symbols
* webfonts - Web Font files used with the CSS
* LICENSES.txt - Nobody with read this


### Usage
The symbols have been divided up into 4 groups: 
* characters - Individual characters
* deprecated - Any symbol marked as _(OLD)
* diacritics - Punctuation, Arabic Numbers, Latin Alphabet and Indicators
* words - Combinations of symbols 

These can be called with a classname within a \<i /> tag. The class names are prefaced with "bs-" and can either be the id or the english translation. 
However, to get the enlgish translation to work as a class name commas have been replaced with hyphens, and parenthesis have been removed entirely.

You can load and use any single or combination of CSS files to allow calling symbols that are broken up into each respective category.


### Example

```HTML
<head>
  <link href="/your-path-to-bliss-font/css/characters.css" rel="stylesheet"> <!--loads all character symbol styles -->
  <link href="/your-path-to-bliss-font/css/deprecated.css" rel="stylesheet"> <!--loads all deprecated symbol styles -->
  <link href="/your-path-to-bliss-font/css/diacritics.css" rel="stylesheet"> <!--loads all diacritic symbol styles -->
  <link href="/your-path-to-bliss-font/css/words.css" rel="stylesheet"> <!--loads all word symbol styles -->
</head>
<body>
  <i class="bs bs-13428"></i> <!-- Loads the court,field_(OLD) symbol -->
  <i class="bs bs-court-field_OLD"></i> <!-- Also loads the court,field_(OLD) symbol -->
</body>
```
