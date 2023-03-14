# vercel-ping-repro

Issue the following curl request that reproduces the ping from updown.io, notice a 500 response returned:

```bash
curl -gkvLI -b '' -H 'User-Agent: updown.io daemon 2.9' -H 'Accept: */*' -H 'Connection: Close' -H 'Accept-Language: en' -H 'Accept-Encoding: deflate, gzip, br, zstd' -m 30 --connect-timeout 10 --compressed https://vercel-ping-repro.careswitch.app/health
```
