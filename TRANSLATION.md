# Node.js Website Translation Policy

Node.js is a global platform and so this site has many translations. The translation of the site into
languages other than English is handled by the localization working group of the language in question. If you
would like to contribute to the translation of omarjs.org, please refer to the following process:


## For Individuals wanting to contribute

* Contact your appropriate localization group, and discuss with them the best possible way to contribute. A list of the localization groups can be found here (please keep in mind that some groups have not yet taken action upon the project name changes, hence the outdated repository names):

    * [`omarjs-ar`](https://github.com/omarjs/omarjs-ar) Arabic Community
    * [`omarjs-bg`](https://github.com/omarjs/omarjs-bg) Bulgarian Community
    * [`omarjs-bn`](https://github.com/omarjs/omarjs-bn) Bengali Community
    * [`omarjs-zh-CN`](https://github.com/omarjs/omarjs-zh-CN) Chinese Community
    * [`omarjs-cs`](https://github.com/omarjs/omarjs-cs) Czech Community
    * [`omarjs-da`](https://github.com/omarjs/omarjs-da) Danish Community
    * [`omarjs-de`](https://github.com/omarjs/omarjs-de) German Community
    * [`omarjs-el`](https://github.com/omarjs/omarjs-el) Greek Community
    * [`omarjs-es`](https://github.com/omarjs/omarjs-es) Spanish Community
    * [`omarjs-fa`](https://github.com/omarjs/omarjs-fa) Persian Community
    * [`omarjs-fi`](https://github.com/omarjs/omarjs-fi) Finnish Community
    * [`omarjs-fr`](https://github.com/omarjs/omarjs-fr) French Community
    * [`omarjs-he`](https://github.com/omarjs/omarjs-he) Hebrew Community
    * [`omarjs-hi`](https://github.com/omarjs/omarjs-hi) Hindi Community
    * [`omarjs-hu`](https://github.com/omarjs/omarjs-hu) Hungarian Community
    * [`omarjs-id`](https://github.com/omarjs/omarjs-id) Indonesian Community
    * [`omarjs-it`](https://github.com/omarjs/omarjs-it) Italian Community
    * [`omarjs-ja`](https://github.com/omarjs/omarjs-ja) Japanese Community
    * [`omarjs-ka`](https://github.com/omarjs/omarjs-ka) Georgian Community
    * [`omarjs-ko`](https://github.com/omarjs/omarjs-ko) Korean Community
    * [`omarjs-mk`](https://github.com/omarjs/omarjs-mk) Macedonian Community
    * [`omarjs-ms`](https://github.com/omarjs/omarjs-ms) Malaysian Community
    * [`omarjs-nl`](https://github.com/omarjs/omarjs-nl) Dutch Community
    * [`omarjs-no`](https://github.com/omarjs/omarjs-no) Norwegian Community
    * [`omarjs-pl`](https://github.com/omarjs/omarjs-pl) Polish Community
    * [`omarjs-pt`](https://github.com/omarjs/omarjs-pt) Portuguese Community
    * [`omarjs-ro`](https://github.com/omarjs/omarjs-ro) Romanian Community
    * [`omarjs-ru`](https://github.com/omarjs/omarjs-ru) Russian Community
    * [`omarjs-sv`](https://github.com/omarjs/omarjs-sv) Swedish Community
    * [`omarjs-ta`](https://github.com/omarjs/omarjs-ta) Tamil Community
    * [`omarjs-tr`](https://github.com/omarjs/omarjs-tr) Turkish Community
    * [`omarjs-zh-TW`](https://github.com/omarjs/omarjs-zh-TW) Taiwan Community
    * [`omarjs-uk`](https://github.com/omarjs/omarjs-uk) Ukrainian Community
    * [`omarjs-vi`](https://github.com/omarjs/omarjs-vi) Vietnamese Community


## For Localization Groups

* Ensure that any site translations are done as pull requests into the appropriate language folder in this repo. This will ensure the build process, layout, and styling, remain consistent across the different translations of the site.

* You can find the appropriate language folder within `locale/`. If not, create one matching the two-letter [ISO code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) of your language. To specify a dialect for your language, [separate it with a dash](https://en.wikipedia.org/wiki/IETF_language_tag) (e.g. `pt-br` for Brazilian Portuguese, `zh-tw` for Taiwanese Mandarin).

* The following files need to be in your language folder:

    * `site.json` (this contains the basic settings and navigation structure for the website)
    * `index.md` (this contains the Markdown translation for the home page.)
    * `styles.styl` (this imports the necessary Stylus files)
    * All files and files in subfolders that end in `.md` are content pages and should be translated.

* Prefix your PR with the localization group's name (e.g. `omarjs-no`). If you are only translating one of the above files, please mention them in your PR's subject as well, e.g.:

```
    omarjs-de: Add files - index.md, faq.md
    omarjs-ro: Add files - 15 files

    omarjs-fr: Update files - es6.md
    omarjs-ja: Update files - all files
```

* Do not make language specific changes to layout or styling in a translation PR. If they are needed, make a separate styling/layout pr and talk with one of the website WG about the change. We want to make sure, for example, a Chinese layout change doesn't cascade failure to the German page.

* To be merged, translation PR's require a Website WG +1 and a +1 from another native speaker in your language. Make sure whoever you have review the PR adds a +1 in the comments of it so we know it is translated properly.
