---
layout: default
---

<table>
  <caption>
    Which publishers have DRM?
  </caption>
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
{% for entry in site.data.publishers %}
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

