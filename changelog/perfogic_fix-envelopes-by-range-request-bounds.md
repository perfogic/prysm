### Fixed

- `ExecutionPayloadEnvelopesByRange`: reject requests with `count` above `MAX_REQUEST_PAYLOADS` instead of serving the last envelopes of the range, and serve nothing for a range that starts after the current slot or ends before the Gloas fork instead of an envelope outside the requested range.
- Bound outgoing `ExecutionPayloadEnvelopesByRange` requests to `MAX_REQUEST_PAYLOADS`, shortening the initial-sync payload range and its block batch when the batch is wider.
