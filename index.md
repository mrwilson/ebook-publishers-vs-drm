---
layout: default
---

<table>
  <thead>
    <tr>
      <th scope="col">Name</th>
      <th scope="col">Region(s)</th>
      <th scope="col">Sells Ebooks</th>
      <th scope="col">DRM-free</th>
      <th scope="col">Notes</th>
    </tr>
  </thead>
  <tbody>
{% assign publishers = site.data.publishers | sort: "publisher_name" %}
{% for entry in publishers %}
    <tr>
      <th scope="row"><a href="{{ entry.publisher_url }}">{{ entry.publisher_name }}</a></th>
      <td>{{ entry.publisher_region }}</td>
      <td>{% if entry.sells_ebooks == "true" %}✅{% else %}❌{% endif %}</td>
      <td>{% if entry.sells_drm_free_ebooks == "true" %}✅{% else %}❌{% endif %}</td>
      <td>{{ entry.notes }}</td>
    </tr>
{% endfor %}
  </tbody>
</table>

Download the raw data as <a href="https://github.com/mrwilson/ebook-publishers-vs-drm/blob/main/_data/publishers.csv">CSV</a> or <a href="{{ site.url }}/data.json">JSON</a>

