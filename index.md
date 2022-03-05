## Welcome to Juno's NFT list

You can use the [editor on GitHub](https://github.com/hippietechies/nftjuno/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### NFTs

{% assign work_items = site.work_items | sort: 'date' | reverse %}
{% for work_item in work_items limit:4  %}
  <div>
      <a href="{{ work_item.url | prepend: site.baseurl }}">{{ work_item.title }}</a>
  </div>
{% endfor %}