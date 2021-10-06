## Final BBH Graphs

You can use the [editor on GitHub](https://github.com/gbooyay/test/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.
[this is a link](https://github.com/gbooyay/test/blob/main/0.900049-0.930145.html)

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/gbooyay/test/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

var filterManager = new FilterManager({
    el:'#filters',
    filterSettings: {
        visibleFilters: ['parameter1', 'parameter2']
    },
});
var graph = new graphly.graphly({
    el: '#graph',
    renderSettings: {
        xAxis: 'parameter1',
        yAxis: ['parameter2', 'parameter3'],
        y2Axis: ['parameter4']
    },
    filterManager: filterManager
});

graph.loadData({
    parameter1: [1, 2, 3, 4],
    parameter2: [0.1, 0.2, 0.3, 0.4],
    parameter3: [0.4, 0.3, 0.2, 0.1],
    parameter4: [150, 100, 120, 130]
});

<iframe width="900" height="800" frameborder="0" scrolling="no" src="//plotly.com/~gbooyay/5.embed"></iframe>
