# krusader-minify-code
User actions for Krusader file manager to minify JS and CSS files on-the-fly (With right mouse click)

## HOW TO USE
First, download and save
[Krusader user actions XML file](https://raw.githubusercontent.com/jontofly/krusader-minify-code/master/krusader-code-minify-user-actions.xml)

Then (Either Option):
* Option A
  * In Krusader's menu, "Useractions" -> "Manage User Actions" -> "Import useractions" -> Choose the "krusader-code-minify-user-actions.xml" file.
* Option B
  * Embed the text from the XML file into your Krusader's one.
* Option C
  * Manually create / edit a user action using these commands:
  * For CSS
    * `curl -X POST -s --data-urlencode 'input@%aCurrent%' http://cssminifier.com/raw > %_Ask("New minified name:", %aCurrent%)%`
  * For JS
    * `curl -X POST -s --data-urlencode 'input@%aCurrent%' http://javascript-minifier.com/raw > %_Ask("New minified name:", %aCurrent%)%`

That's it.

### NOTE
Needs "cURL" installed to function.

### CREDITS
Thanks to
* [Krusader Developers](http://www.krusader.org/.) - Twin Panel [Orthodox file manager](https://en.wikipedia.org/wiki/Orthodox_file_manager) File Manager.
  * [Krusader Wiki Page](https://en.wikipedia.org/wiki/Krusader)
* [Andrew Chilton AKA chilts](https://github.com/chilts) - Code Minify API.
  * [CSS Minifier](http://cssminifier.com/)
  * [Javascript Minifier](http://javascript-minifier.com/)
