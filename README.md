**Cankarjev dom API**
----
  Returns the list of events for the requested month.

* **URL**

  https://www.cd-cc.si/koledar/mesec/$month/all

* **Method:**
  
  `GET`

  
*  **URL Params**

   <_$month = requested month e.g. https://www.cd-cc.si/koledar/mesec/01-06-2019/all for June 2019_> 
 
* **Success Response:**
  
  <_The events object contains all the days in the month, each day can contain multiple event objects, sorted by the start time of the show (if available).  _>

  * **Code:** 200 <br />
    **Content:**
    
| Field   |      Type      |  Description |
|----------|:-------------:|------:|
| title |  string | The title of the event. |
| times |    string   |   The start time of the event. In case of full day events, the value is always 23:59 |
| url | string |    Relative URL of the event |
| full_url | string |    Absolute URL of the event  |
| day | string |    The day of the event, used internally. Can be empty.  |
| multiple_day | boolean |    Indicates a multiple day event e.g. an exhibition.  |
| description | string |    Short description of the event.  |
| category | string |    The main category of the event e.g. Music, Cinema, ...  |
| hall | string |    The hall where the event takes place.  |
| image_desktop | string |    The URL to the large (desktop) version of the main event image (hero image).  |
| price | string |    The price of the event.  |
| full_description | string |    Long description of the event. Contains HTML.  |

```json
{
  "events": {
    "1": {
      "event": [
        {
          "title": "Dance amore: Zapleši ljubezen"
          , "times": "20:00"
          , "url": "/kultura/gledalisce-in-ples/dance-amore-zaplesi-ljubezen"
          , "full_url": "https://www.cd-cc.si/kultura/razstave/franc-solina-enej-gucek-puhar-empatija"
          , "day": "Sobota"
          , "multiple_day": false
          , "description": "Plesna uspešnica v bleščečem soju Broadwaya se vrača v Cankarjev dom!\r\nPrireja: GIG INT, prireditvena agencija, d.o.o."
          , "category": "Razstave"
          , "hall": "Trg republike (pri Cankarjevem spomeniku)"
          , "image_desktop": "https://www.cd-cc.si/sites/www.cd-cc.si/files/images/hero/solina_gucek_empatija.png"
          , "price": "Prosti vstop"
          , "full_description": "<p>Koprodukcija: Strip Core/Forum Ljubljana in Cankarjev dom<br />Odprtje bo v četrtek, 16. maja, ob 21.30</p><p> </p><p>Empatija je značajska kategorija, s katero opisujemo zmožnost posameznika, da se vživi in razume sočloveka; lahko jo razumemo kot nekakšno prečenje čustvenih meja med posamezniki. Interaktivna projekcija skuša vizualizirati tovrstne odnose med ljudmi, pri čemer za svoje delovanje zahteva empatične posameznike. Infrardeča kamera v prostoru globinsko zaznava gibanje ljudi in jih s pomočjo programskih orodij pretvarja v projicirane človeške silhuete. Če se ljudje na dosegu kamere dotikajo, če si izkazujejo fizično naklonjenost, se na projekciji pojavi zanimiv vizualni učinek, ki s pomočjo dinamike barvnih krogov na simboličen način ponazarja empatijo med ljudmi, vzpostavljanje novih prijateljskih vezi med njimi.</p><p>Več inforamacij o dogodkih festivala na www.svetlobnagverila.net</p>"
          , "image_mobile": "https://www.cd-cc.si/sites/www.cd-cc.si/files/images/hero/svetlobna_gverila_meje_m.jpg"
        }],
        "day": "Sobota
    }
  }
}
```
