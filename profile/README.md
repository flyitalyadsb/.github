# FlyItalyADSB

A global community network, born in Italy in 2020, with about 3,200 receivers: they send us
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
What feeding gets you:

- **The API with Pro limits, free:** 300 requests a minute, 10 million a month, the whole
  world, on your Free keys, for non-commercial use. [Turn it on in My API](https://flyitalyadsb.com/en/data/api/account/?utm_source=github&utm_campaign=org-profile)
  from your receiver's network.
- **What flew past you:** [Lightcone](https://flyitalyadsb.com/en/community/lightcone/?utm_source=github&utm_campaign=org-profile) shows the aircraft
  that passed near you and your receiver did not receive, and how you compare with the
  receivers within 40 km. graphs1090 and tar1090 only show what you received.

Set it up with ultrafeeder following the [feeder guide](https://flyitalyadsb.com/en/community/feeder/?utm_source=github&utm_campaign=org-profile).
If your receiver already runs a decoder, the [fly-italy-adsb](https://github.com/flyitalyadsb/fly-italy-adsb)
script adds the feed and MLAT.

## Repositories

| Repository | What it is |
|---|---|
| [adsb-api](https://github.com/flyitalyadsb/adsb-api) | API quickstart, examples, OpenAPI spec, `llms.txt` |
| [fly-italy-adsb](https://github.com/flyitalyadsb/fly-italy-adsb) | Install script for feeders |
| [readsb](https://github.com/flyitalyadsb/readsb), [tar1090](https://github.com/flyitalyadsb/tar1090), [mlat-server](https://github.com/flyitalyadsb/mlat-server), [mlat-client](https://github.com/flyitalyadsb/mlat-client) | Our forks of the open-source decoder, map and MLAT tools |
| [flarm-ogn-to-sbs](https://github.com/flyitalyadsb/flarm-ogn-to-sbs) | FLARM/OGN glider data as an SBS stream |

[Live map](https://map.flyitalyadsb.com/?utm_source=github&utm_campaign=org-profile) ·
[Status](https://flyitalyadsb.com/en/status/?utm_source=github&utm_campaign=org-profile) ·
[Facts as JSON](https://flyitalyadsb.com/facts.json) ·
[Contact](https://flyitalyadsb.com/en/contact/?utm_source=github&utm_campaign=org-profile)

Run by Nesso Labs S.r.l., Brescia, Italy.

<details>
<summary>In italiano</summary>

Rete community globale, nata in Italia nel 2020, con circa 3.200 ricevitori: ci mandano i
dati direttamente, ADS-B e la nostra multilaterazione (MLAT), aperti e non filtrati. Mappa live gratuita, API REST e server MCP per gli assistenti AI.

**Per chi costruisce prodotti.** Posizioni di circa 11.000 aerei, aggiornate ogni 2 secondi,
per qualsiasi punto della Terra; militari, PIA e LADD compresi. L'API si può usare in un
prodotto che vendi con ogni piano, Free compreso, con una riga di attribuzione (CC BY-SA 4.0).
Free e Starter coprono la tua zona (500 e 1.000 km); **Pro: il mondo intero in una
richiesta, €49 al mese.** Oltre i limiti ricevi un 429 o un 403, mai costi extra.
[Chiave gratuita e documentazione](https://flyitalyadsb.com/dati/api/?utm_source=github&utm_campaign=org-profile).

**Per i feeder.** La rete è fatta di ricevitori come il tuo (un Raspberry Pi e una chiavetta
RTL-SDR, circa €55–110). Mandandoci i dati hai in più:

- **l'API con i limiti Pro, gratis:** 300 richieste al minuto, 10 milioni al mese, tutto il
  mondo, sulle tue chiavi Free, per uso non commerciale. [Attivali da La mia API](https://flyitalyadsb.com/dati/api/account/?utm_source=github&utm_campaign=org-profile)
  dalla rete del ricevitore;
- **cosa ti è passato accanto:** [Lightcone](https://flyitalyadsb.com/community/lightcone/?utm_source=github&utm_campaign=org-profile) mostra gli aerei
  passati vicino a te che il tuo ricevitore non ha ricevuto e come vai rispetto ai ricevitori
  entro 40 km. graphs1090 e tar1090 mostrano solo cosa hai ricevuto.

Si configura con ultrafeeder seguendo la [guida per i feeder](https://flyitalyadsb.com/community/feeder/?utm_source=github&utm_campaign=org-profile).
Se il ricevitore ha già un decoder, lo script [fly-italy-adsb](https://github.com/flyitalyadsb/fly-italy-adsb)
aggiunge il feed e la MLAT.

</details>
