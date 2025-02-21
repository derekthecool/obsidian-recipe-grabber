This plugin allows you to paste the url of any recipe into your Obsidian page and get the contents in a concise recipe format along with the image and link back to the original page.

Its built for those of you who want to save the recipe, and not the complete history of biscuits and how much the author loves making them on their family trip to Maine.

https://github.com/seethroughdev/obsidian-recipe-grabber/assets/203779/88e3977c-fbb8-4bc6-a770-06071af154d1

---

### Frontmatter Issues

[Obsidian 1.4.6](https://obsidian.md/changelog/2023-08-31-desktop-v1.4.6/) changed the frontmatter behaviour.
The frontmatter has to start on the first line of the file now. If you have leading newlines in your recipe template, the resulting frontmatter won't be properly parsed by obsidian.
If you have this problem, go to the settings of this plugin and remove the leading newlines.

### Custom templating

Prefer your own layout instead? No problem. Just paste a [custom handlebars string template](https://handlebarsjs.com/guide/#simple-expressions) into the settings.

We're assuming the page has a [json recipe](https://developers.google.com/search/docs/appearance/structured-data/recipe#guided-example) on the page. Make sure to check the [Example Recipe](https://developers.google.com/search/docs/appearance/structured-data/recipe#guided-example) for a list of what fields you can pull. And keep in mind that lots of recipes seem to not stick exactly to the spec. So expect some thing to take a little extra effort to get them there.

You can also add `{{{json}}}` for the raw json in the template if you like.

In the meantime, I did my best to make the most recipes I can work out of the box. Please [create ticket](#) if you have suggestions for improving it!
