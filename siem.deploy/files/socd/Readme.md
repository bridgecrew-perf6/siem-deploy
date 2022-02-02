SOC Daemon
==========

The SOC Daemon (socd, for short) is an API gateway that allows to concentrate and abstract various external information sources into a developer-friendly REST API.

It uses [KrakenD](https://www.krakend.io/) as a backend and brings the following advantages:
- Only one endpoint host for all services allowing unauthorized requests from trusted network and hiding service credentials for the commercial services.
- Request caching for limit external requests and save per-requests license costs for commercial services.
- Logging and metrics (of course) for services used to caculate required licenses.
- Aggregating several services into one response to limit the number of requests per enrichment worker.
- Easily configurable endpoints via user-freindly web interface.

