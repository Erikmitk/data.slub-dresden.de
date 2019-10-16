---

layout: default

title: /{authority_provider}
nav_order: 5
parent: "API endpoints"

---

# Query LOD API by searching for authority provider's ID

In case you know the ID of your dataset for one of the listed authority providers, you can use this id
If one only needs results for certain entities the `/{entity_index}` can be used. This makes it possible to look - for example - just for results in organizations or persons.

## Usage

---

/{authority_provider}/`{id}` \\
/{authority_provider}/`{entity_index}`/`{id}`
{: .fs-5.fw-200.text-red-200.mx-auto}

---

It is preferred to use the second call of the API in case you already know the entity index of your dataset, see [`/{entity_index}`]({{ site.baseurl }}{% link doc/api_endpoints/entity_index.md %}), because this call can be processed much faster by elasticsearch compared to the more general request not providing the entity index.

possible values for `{entity_index}`:
* `events`
* `slub-resources`
* `works`
* `organizations`
* `topics`
* `geo`
* `persons`


## Example
```sh
$
```



[Try Me](http://data.slub-dresden.de/api){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .m r-2 }