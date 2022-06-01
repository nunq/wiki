# captive portals

## how it works
if your device uses the default dns servers advertised by the router over dhcp, all (plain http, because its not encrypted) queries are redirected to the terms of service or login page.
your device is then allowed to access the internet. i think these services use your mac address as an identifier that they store to allow you access for N hours.

## problems
if you use another dns server without the gateway dns fallback, you wont reach the captive portal because the advertised dns server is never queried (your own is)

