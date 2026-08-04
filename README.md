# Pelias

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Pelias is a modular, open-source geocoding search engine built on Elasticsearch. It converts addresses and place names into geographic coordinates (forward geocoding) and geographic coordinates into places and addresses (reverse geocoding). Powered entirely by open data, it is available under the MIT license and can be self-hosted or accessed via commercial hosted services.

## API Endpoints

| Endpoint | Path | Description |
|----------|------|-------------|
| Forward Geocoding | `GET /v1/search` | Find a place by address or name |
| Reverse Geocoding | `GET /v1/reverse` | Find what is at a coordinate |
| Autocomplete | `GET /v1/autocomplete` | Real-time suggestions as the user types |
| Structured Geocoding | `GET /v1/search/structured` | Geocode pre-parsed address components |
| Place Lookup | `GET /v1/place` | Retrieve details for a known place GID |

All responses are returned as GeoJSON.

## Data Sources

- OpenStreetMap
- OpenAddresses
- Who's on First
- Geonames
- Polylines
- CSV (custom datasets)

## Deployment

- **Self-hosted**: Use the [Docker setup](https://github.com/pelias/docker) to run Pelias locally or in the cloud.
- **Hosted service**: [Geocode Earth](https://geocode.earth) is the commercial API built by the original Pelias team, with plans starting at $100/month.

## Links

- Website: https://pelias.io
- Documentation: https://github.com/pelias/documentation
- GitHub Organization: https://github.com/pelias
- Hosted Service: https://geocode.earth
- Community Chat: https://gitter.im/pelias/pelias
- Contact: team@pelias.io

## License

MIT License
