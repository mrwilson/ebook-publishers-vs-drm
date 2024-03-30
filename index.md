---
layout: default
---

# Which e-book publishers have DRM?

## Publishers

<table>
  <caption>
    Which publishers have DRM?
  </caption>
  <thead>
    <tr>
      <th scope="col">Name</th>
      <th scope="col">URL</th>
      <th scope="col">Region(s)</th>
      <th scope="col">Sells Ebooks</th>
      <th scope="col">Sells DRM-free Ebooks</th>
      <th scope="col">Notes</th>
    </tr>
  </thead>
  <tbody>
{% for entry in site.data.publishers %}
    <tr>
      <th scope="row">{{ entry.publisher_name }}</th>
      <td>{{ entry.publisher_url }}</td>
      <td>{{ entry.publisher_region }}</td>
      <td>{{ entry.sells_ebooks }}</td>
      <td>{{ entry.sells_drm_free_ebooks }}</td>
      <td>{{ entry.notes }}</td>
    </tr>
{% endfor %}
  </tbody>
</table>

