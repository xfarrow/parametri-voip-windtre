# Parametri VOIP/SIP WindTre
Parametri VOIP/SIP WindTre (ex Infostrada) per connessioni FTTC e FTTH.

Questo ISP sembra non fornire una chiara configurazione SIP, infatti, secondo [il loro forum](https://community.windtre.it/configurazioni%2Dlinea%2Dfissa%2Dfibra%2D15/come%2Dconfigurare%2Dun%2Dmodem%2Dnon%2Dfornito%2Dda%2Dwindtre%2Dfibra%2Dadsl%2De%2Dvoip%2D208) 
per far ciò bisogna chiamare il supporto tecnico

**Avvertenza:** Usare queste informazioni solo in accordo alla legge e in accordo al contratto stipulato con Wind Tre S.p.A.

**Avvertenza DNS:** Il telefono potrebbe non funzionare se vengono cambiati i parametri DNS sul modem/router. Questo avviene perché gli indirizzi mostrati nelle 
tabelle di seguito possono essere risolti solo dal resolver di WindTre. Per ovviare al problema, indicare l'indirizzo IP dei server
anziché indicare l'URI  (es. xxx.xxx.xxx.xxx anziché voip.libero.it) 

## SIP Service Provider

$Menu \rightarrow Voip \rightarrow SIP \rightarrow SIP \ Service \ Provider \rightarrow Edit $

| Parametro | Configurazione |
| --- | --- |
| SIP Proxy Server Address | voip.libero.it |
| SIP Local Port | 5060 |
| SIP Proxy Server Port | 5060 |
| SIP REGISTRAR Server Address | voip.windtre.it |
| SIP REGISTRAR Server Port | 5060 |
| SIP Service Domain | windtre.it |
| Outbound Proxy Address | voip.windtre.it |
| Outbound Proxy Port | 5060 |
| Use DHCP Option 120 First | False |
| PRACK (RFC 3262, Require: 100rel) | True |
| Don't send re-Invite to the remote party when there are multiple codecs answered in the SDP | True |
| Replace dial digit '#' to '%23' in SIP messages | True |
| Remove the 'Route' header in SIP messages | True |
| RTP Start Port | 50001 |
| RTP End Port | 50016 |
| SRTP Support | False |
| DTMF Mode | RFC 2833 |
| Transport Type | UDP |
| Ignore Direct IP | Disable |
| FAX Option | G.711 Fax Passthroug |
| SIP DSCP Mark Setting | 46  |
| RTP DSCP Mark Setting | 0   |
| SIP Register Expiration Duration | 3600 |
| SIP Register Fail Re-try Timer | 32  |
| Session Expires (SE) | 3600 |
| Min-SE | 90  |

## SIP
$Menu \rightarrow Voip \rightarrow SIP \rightarrow Edit $

| Parametro | Configurazione |
| --- | --- |
| Enable SIP Account | True |
| Username | \[ Chiamare il 159 \] |
| Password | \[ Chiamare il 159 \] |
| URL Type | SIP |
| Primary Compression Type | G.729 |
| Secondary Compression Type | G.711a |
| Third Compression Type | G.711u |
| Enable Call Waiting | True |
