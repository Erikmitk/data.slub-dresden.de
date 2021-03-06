---
layout: default

title: API endpoints
description: "endpoints or functions provided by the API"
nav_order: 3
has_children: true
permalink: doc/api_endpoints
---

# How to query the API
  The API is used through its endpoints. Depending on the task at hand some endpoints are better suited than others. You can also have a look at the comprehensive [Swagger UI](https://data.slub-dresden.de/doc/api){: .extlink }.

[Try Me](https://data.slub-dresden.de/doc/api){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .m r-2 }

## Search for an entry
   The endpoint [`/search`]({{ site.baseurl }}{% link doc/api_endpoints/search.md %}) provides an interface for searching through all resources

## Query one source index (SWB, K10Plus) directly
   The endpoint [`/source`]({{ site.baseurl }}{% link doc/api_endpoints/source.md %}) realizes a direct interface to the (unprocessed) source datasets located in different source indices. A dataset can be requested with its index-specific ID.

## Query datasets by its entity ('persons', 'organizations', 'events', …)
   The endpoint [`/{entity_index}`]({{ site.baseurl }}{% link doc/api_endpoints/entity_index.md %}) gives the possibility to query only specified entities.

## Query an ID used by an authority provider (GND, wikidata, SWB, …)
   The endppoint [`/{authority_provider}`]({{ site.baseurl }}{% link doc/api_endpoints/authority_provider.md %}) are used to query one dataset by its ID provided by authority providers like GND, wikidata, or SWB.

## Connect via OpenRefine reconciliation API
   The endpoint [`/reconcile`]({{ site.baseurl }}{% link doc/api_endpoints/reconcile.md %}) can be used with Google's OpenRefine.


# Limitations

   Our API is not suited for bulk-download of data. It will not return more than 10'000 results.
