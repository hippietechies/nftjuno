---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
{% assign nfts = site.data.nfts | sort: 'launchdate' | reverse %}

{% for nft in nfts %}
  <div style="align:center">
    <a href="{{ nft.name | prepend: nft.link }}">
      <img width="50" height="50" src="{{ nft.icon_link }}">{{ nft.name }}
      <img src="{{ nft.banner_link }}">
    </a>
    <br />
    <br />
  </div>
{% endfor %}
