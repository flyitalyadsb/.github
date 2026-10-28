# FlyItalyADSB

A community network born in Italy and now global: about 3,200 receivers worldwide send us
their data directly, ADS-B and our own multilateration (MLAT), open and unfiltered.
A free live map, a REST API and an MCP server for AI assistants.

## For people building products

- Live positions of about 11,000 aircraft, updated every 2 seconds, for any point on Earth.
- Unfiltered: military, PIA and LADD aircraft are included.
- You can use the API in a product you sell on every plan, Free included, with one
  attribution line (CC BY-SA 4.0).
- Free and Starter cover your area (500 and 1,000 km). **Pro: the whole world in one
  request, €49 a month.**
- Over the limits you get a 429 or 403, never an extra charge.

```bash
curl -H "X-Api-Key: $FLYITALYADSB_KEY" \
  https://api.flyitalyadsb.com/v2/lat/40.64/lon/-73.78/dist/50
```

[Free API key](https://flyitalyadsb.com/en/data/api/?utm_source=github&utm_campaign=org-profile#api-key) ·
[Docs](https://flyitalyadsb.com/en/data/api/docs/?utm_source=github&utm_campaign=org-profile) ·
[OpenAPI 3.1](https://flyitalyadsb.com/openapi.json) ·
[MCP server](https://flyitalyadsb.com/en/data/mcp/?utm_source=github&utm_campaign=org-profile) ·
[Examples in curl, Python, Node.js and ESP32](https://github.com/flyitalyadsb/adsb-api)

Code written for the ADS-B Exchange v2 API works with a new host and key.

## For feeders

The network is made of receivers like yours (a Raspberry Pi and an RTL-SDR, about €55–110).
[fly-italy-adsb](https://github.com/flyitalyadsb/fly-italy-adsb) sends your data and MLAT to
us: see the [feeder guide](https://flyitalyadsb.com/en/community/feeder/?utm_source=github&utm_campaign=org-profile).
[Lightcone](https://flyitalyadsb.com/en/community/lightcone/?utm_source=github&utm_campaign=org-profile)
then shows how many of the aircraft the network saw near you your receiver got, and how it
compares with the receivers around it.

## Repositories

| Repository | What it is |
|---|---|
| [adsb-api](https://github.com/flyitalyadsb/adsb-api) | API quickstart, examples, OpenAPI spec, `llms.txt` |
| [fly-italy-adsb](https://github.com/flyitalyadsb/fly-italy-adsb) | Install script for feeders |
| [readsb](https://github.com/flyitalyadsb/readsb), [tar1090](https://github.com/flyitalyadsb/tar1090), [mlat-server](https://github.com/flyitalyadsb/mlat-server), [mlat-client](https://github.com/flyitalyadsb/mlat-client) | Our forks of the open-source decoder, map and MLAT tools |
| [flarm-ogn-to-sbs](https://github.com/flyitalyadsb/flarm-ogn-to-sbs) | FLARM/OGN glider data as an SBS stream |

[Live map](https://mappa.flyitalyadsb.com/?utm_source=github&utm_campaign=org-profile) ·
[Status](https://flyitalyadsb.com/en/status/?utm_source=github&utm_campaign=org-profile) ·
[Facts as JSON](https://flyitalyadsb.com/facts.json) ·
[Contact](https://flyitalyadsb.com/en/contact/?utm_source=github&utm_campaign=org-profile)

Run by Nesso Labs S.r.l., Brescia, Italy.

<details>
<summary>In italiano</summary>

Rete community nata in Italia e oggi globale: circa 3.200 ricevitori in tutto il mondo ci
mandano i dati direttamente, ADS-B e la nostra multilaterazione (MLAT), aperti e non
filtrati. Mappa live gratuita, API REST e server MCP per gli assistenti AI.

**Per chi costruisce prodotti.** Posizioni di circa 11.000 aerei, aggiornate ogni 2 secondi,
per qualsiasi punto della Terra; militari, PIA e LADD compresi. L'API si può usare in un
prodotto che vendi con ogni piano, Free compreso, con una riga di attribuzione (CC BY-SA 4.0).
Free e Starter coprono la tua zona (500 e 1.000 km); **Pro: il mondo intero in una
richiesta, €49 al mese.** Oltre i limiti ricevi un 429 o un 403, mai costi extra.
[Chiave gratuita e documentazione](https://flyitalyadsb.com/dati/api/?utm_source=github&utm_campaign=org-profile).

**Per i feeder.** La rete è fatta di ricevitori come il tuo (un Raspberry Pi e una chiavetta
RTL-SDR, circa €55–110). [fly-italy-adsb](https://github.com/flyitalyadsb/fly-italy-adsb)
ci manda i tuoi dati e la MLAT: la [guida per i feeder](https://flyitalyadsb.com/community/feeder/?utm_source=github&utm_campaign=org-profile).
[Lightcone](https://flyitalyadsb.com/community/lightcone/?utm_source=github&utm_campaign=org-profile)
ti mostra quanti degli aerei che la rete ha visto vicino a te ha ricevuto il tuo ricevitore,
e come va rispetto ai ricevitori intorno.

</details>
