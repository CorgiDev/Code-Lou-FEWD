# Wiki Specific Documentation

## Using the Wiki
Start by opening the `mdwiki.html` file. It should automatically append `#!index.html` to the end of the URL to access the homepage. If not, add that to the end to view the home page and then navigate the rest as normal.

**IMPORTANT:** NEVER change the `mdwiki.html` file except for if you want to change the `<title>`.

## Editing the Wiki
Look at other pages for structure to try to keep things kind of consistent. The `mdwiki.html` file needs to be at the root. It in turn is what causes the rest of the md files stored in its folder to be viewable.

### Markdown Format
It uses *GitHub* style Markdown with some special tricks you can make use of (i.e. floating images to the left or right, while allowing text to of to the other side.) and addons you can add to it referred to as *Gimmicks*.

### Navigation
The nav menu at the top of the page is controlled by the `navigation.md` file.

Want a sort of table of contents for an individual page? Make just the first header an H1 header. Then every H2 header you add will be added to an automatically generated table of contents.

### Additional Formatting Information
The [Quick Start](http://dynalon.github.io/mdwiki/#!quickstart.md) and [LayOut](http://dynalon.github.io/mdwiki/#!layout.md) pages on the official MDwiki page provide additional details about formatting and editing.

##  Issues opening locally
**Q:** Can I open mdwiki.html in my browser from the menu or by specifying via a file:// URL?
**A:** Yes, at least for most browsers. There are some gimmicks that won't work on some browsers. List of browser that support opening MDwiki via `file://` urls:
- **Firefox (v23):** Works good, no issues known.
- **Internet Explorer (v10):** Works good, no issues known.
- **Google Chrome:** Works only when started with the commandline parameter `--allow-file-access-from-files`. Even then, Chrome has minor issues. I.e. the math gimmick will not render correctly.
- **Safari:** Does not work. Maybe cmdline flag needed as in Chrome?

**Note:** It is usally best to use a webserver when running locally and not to use `file://` URLs as those are not yet 100% supported by every gimmick or third-party script.

Gimmicks that won't work when using `file://` urls:
- Facebok Likebutton (problem with their Cross-Origin setting?)
- Disqus (hardcoded //-prefixed urls in their scripts)

## Additional Details
More details on this and other issues can be found on the [MDwiki FAQ](http://dynalon.github.io/mdwiki/#!faq.md) page.