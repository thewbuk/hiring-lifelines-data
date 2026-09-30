# hiring-lifelines data

Per-company job posting lifelines, rebuilt nightly. This branch is one orphan commit that is
force-pushed on every build; do not base work on it.

- `c/{board}/{company}.json.gz`: every posting the crawler has recorded for one careers board, with
  the day it was first seen and the day it was removed
- `index/{prefix}.json`: search index, sharded by the first two characters of the name and slug
- `meta.json`: build date, ledger date, counts

## Source and licence

Derived entirely from the crawl ledger published by
[elliottdehn/open-jobs](https://github.com/elliottdehn/open-jobs), which is released under
[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). These derived files are released
under CC0 1.0 as well. Thank you to Elliott Dehn for running the crawler and giving the data away.

The `dark` board (career sites discovered by domain, which includes job aggregators) is excluded.
