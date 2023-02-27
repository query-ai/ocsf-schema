
Query extension is added in Query directory instead of extensions folderso that changes are additive only
and can be applied to other extensions with minimal change

## Extending the Schema

Extensions are additional categories, event classes, attributes, objects or profiles. The Open
Cybersecurity Schema Framework can be extended by adding new attributes, objects, categories
and event classes. A schema is the aggregation of core schema entities and extensions.
Extensions allow a particular vendor or customer to create a new schema or augment an existing
schema. Extensions can also be used to factor out non-essential schema domains keeping a
schema small. 

Query extension can be use to extend events, objects, attributes of any of the namespace schema.
namespace is an optional attribute in events, objects, includes which can be added to extend an extension's schema.


| Name              | Description                                                               |
|-------------------|---------------------------------------------------------------------------|
| `categories.json` | Create it to define new categories. Note, to avoid collisions with the categories defined in the core schema, the category IDs must be greater than or equal to 30. |
| `dictionary.json` | Create it to define new attributes.                                       |
| `enums`           | Create it to define new enumerations.                                     |
| `events`          | Create it to define new event classes.                                    |
| `includes`        | Create it to define new shared data.                                      |
| `objects`         | Create it to define new objects.                                          |


## Versioning

Updates to OCSF follow [semantic versioning](https://semver.org/).

## License

This software is licensed under the Apache License, version 2 ("ALv2").
