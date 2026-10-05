# Delfino Modern GitHub 011

# Eiscafé Delfino – GitHub Version 011

Verkaufsfähige Demo mit echtem, getrenntem Supabase-Testbackend.

## Enthalten
- Moderne responsive Startseite
- Speisekarte und Warenkorb auf derselben Website
- Preise werden beim Laden aus Supabase gelesen
- Testbestellungen werden serverseitig gespeichert
- Der Browser kann Preise/Summen nicht festlegen; Supabase berechnet alles erneut aus geschützten Produktvarianten
- Geschützter interner Betriebsbereich `betrieb.html`
- Live-Bestellungen, Statusworkflow, Browser-Benachrichtigungen und Küchenbon-Druck
- Noch keine Online-Zahlung
- GitHub-Modus ist bewusst als Testbestellung gekennzeichnet

## Sicherheit
Die öffentliche Supabase-Publishable-Key ist absichtlich öffentlich und nur für RLS-geschützte Daten vorgesehen.
Bestellungen werden ausschließlich über die Edge Function `place-order` angenommen.
Der Service-/Secret-Key befindet sich niemals in dieser ZIP.

## Betrieb
`betrieb.html` ist nicht auf der Kundenseite verlinkt. Ohne gültigen Supabase-Login und aktives `staff_profiles`-Profil sind keine Bestellungen sichtbar.

Version: 011


## Version 011
- Aktuelle Instagram Spezialkarte mit 10 Empfehlungen integriert und direkt bestellbar.
- Startseite auf „Seit 2008“ aktualisiert.
- Backend Preise der neuen Empfehlungen liegen serverseitig in Supabase.
- favicon.svg und site.webmanifest ergänzt, damit alle lokalen Referenzen vollständig sind.


## Bestellzeiten-Schutz (011)
- Online-Bestellungen serverseitig nur Dienstag–Sonntag 11:30–20:30 Uhr.
- Montag geschlossen.
- Abholzeiten werden ebenfalls gegen den Wochenplan geprüft.
- Sonder-Schließtage können in Supabase gepflegt werden.
- Außerhalb der Zeiten erscheint auf der Speisekarte ein deutlicher Hinweis; der Checkout ist gesperrt.
