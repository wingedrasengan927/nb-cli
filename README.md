## How is varies from the official version

- In the official version, while in `connect` mode, all metadata except `{"trusted": true/false}` is filtered out when adding a new cell. This version ensures that all metadata is retained.
- Another change has been made to make it simpler to add metadata while inserting a cell. Usage:
```bash
nb cell add <notebook-name> -t markdown -s "# Heading" --metadata '{"my_key": "my_value"}'
```