# togostanza-data

## Tree data
[sample JSON file](samples/json/tree-data.json)

[sample TSV file](samples/tsv/tree-data.tsv)

**details:**
* Unique ID for each item
* If the item has children, the children are set as a list of IDs
* If the item is a child itself, the parent is set by its unique ID


**example:**

```JSON
[
  {
    "id": 1,
    "label": "Transcript variant",
    "children": [2, 19, 25, 29, 30]
  },
  {
    "id": 2,
    "label": "Coding variant",
    "children": [3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18],
    "parent": 1
  }
]
```

## Named Map Data
[sample JSON file](samples/json/named-map-data.json)

[sample TSV file](samples/tsv/named-map-data.tsv)

**details:**

  - Countries are identified by the three-digit <a href="https://en.wikipedia.org/wiki/ISO_3166-1_numeric">ISO 3166-1 numeric country code</a>, such as "528"

**example:**
```JSON
[
  {
    "id": "528",
    "rate": "0.9"
  },
  {
    "id": "8",
    "rate": "0.2"
  }
]
```