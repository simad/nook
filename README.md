## Development

To run the site locally, simply run:

```bash
hugo server -D
```

Now you can visit [`localhost:1313`](http://localhost:1313/) to see the site.

### Open Graph Images

If you wish to render open graph images, you can use the following commands:

```bash
npm install
script/images
```

Then copy the resulting PNGs that got generated from the front matter of your blog posts into their corresponding `content/posts/<post-name>` directories.

The text on the open graph images comes from the following front matter fields of a blog post:

```yaml
ogTitle: Grant Birkinbine
ogDescription: "An example of using the Dario hugo theme"
```

After you drop the resulting PNGs into your `content/posts/<post-name>` directories, you can point the following front matter field to the PNG file:

```yaml
ogImage: /posts/example/og.png
```
