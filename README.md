## Graylog content pack for HAProxy

This content pack will launch an UDP input on port 11002 that is able to parse the standard HAProxy HTTP logs. Example log message:

    haproxy[12345]: 92.211.35.123:58507 [10/Jul/2014:08:15:48.478] fe-https-in~ backend1/server2 2055/0/0/160/2215 200 8638 - - ---- 1/1/0/1/0 0/0 "GET / HTTP/1.1"

Will extract fields `backend`, `frontend`, `http_version`, `message`, `remote_addr`, `request_past`, `request_verb`, `response_bytes`, `response_status`, `server`, `tc`, `tq`, `tr`, `tt`, `tw` and `timings`.
