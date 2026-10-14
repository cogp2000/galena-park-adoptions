# Galena Park Kennel — easy editing version

The front-end design is unchanged.

## Edit dogs only in `dogs.txt`
Each dog is one line:

`name|image|age|sex|weight|breed|fixed|microchip|heartworm|status|traits|labels|card text|bio`

Examples: `8 months`, `1 year`, `3 years`; microchip = `yes`/`no`; heartworm = `positive`/`negative`; status = `available`/`pending`; traits = `dog-friendly`, `calm`, `treatment`. Separate multiple traits or labels with commas.

To add a dog: upload its image to `images/`, add one line to `dogs.txt`, commit and push. The inquiry dropdown now updates automatically.

To remove a dog: delete its line from `dogs.txt`, commit and push.

Do not use the `|` character inside descriptions because it separates fields.
