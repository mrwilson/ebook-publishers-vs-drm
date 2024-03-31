# ebook-publishers-vs-drm
List of publishers and whether they sell DRM-free ebooks or not.

## Contributing

The data that powers this site is contained in [_data/publishers.csv](./_data/publishers.csv).

You should include the following information when raising a pull request to add a row to the data source:

- `publisher_name`: Name of the publisher e.g. Really Good Books
- `publisher_url`: URL of the publisher's website
- `publisher_region`: Region in which the publisher sells, or "world" if global
- `sells_ebooks`: This publisher does (`true`) or does not (`false`) sell ebooks
- `sells_drm_free_ebooks`: This publisher does (`true`) or does not (`false`) sell ebooks that do not have DRM
- `notes`: Any additional notes, such as a quote from the publisher with their DRM position
