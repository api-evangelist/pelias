# Pelias

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
