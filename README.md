TensegrityOrientationFetcherV4

Small client-side prototype that demonstrates crawling-like behavior in the browser. Paste or type a list of file URLs (CSV/JSON/ZIP). The page will attempt to fetch each URL, detect file type, parse CSV or JSON, look for likely orientation/pose fields (names like x,y,z,roll,pitch,yaw,quat*), and produce a normalized JSON and CSV export with provenance (source URL, original filename, detected fields).

This is a proof-of-concept only: no server, no credentials. ZIP handling relies on browser support and JS; large files may fail. Use reasonable test files and same-origin or CORS-enabled URLs.

Files:
- index.html : interactive interface and all logic (single-file).