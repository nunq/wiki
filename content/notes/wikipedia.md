# wikipedia

## export wikipedia app reading list
* go into the android app, select the list and click 'Export List' in the three-dot menu

get the urls using:
```sh
jq -r '.readingListsV1[].pages[] | "https://\(.lang).wikipedia.org/wiki/\(.title)"' export.json
```
