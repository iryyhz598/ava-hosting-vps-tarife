# vserver mieten bei AVA Hosting: Welcher Tarif reicht? Was ist im Preis enthalten – und wo sind die Grenzen? Alle Tarife ab 5 €/Monat im Vergleich

Der günstigste monatlich abgerechnete Tarif bei AVA Hosting ist der VPS One für 5 € im Monat: 1 vCPU, 2 GB RAM, 25 GB NVMe. Damit läuft eine Website, ein Discord-Bot, ein Testsystem oder eine kleine Nextcloud. Wer Docker mit mehreren Containern, einen Shop oder eine Datenbank mit echtem Working-Set betreibt, braucht mindestens den VPS Basic für 10 € (2 vCPU, 4 GB, 50 GB); ab 20 € wird es mit dem VPS Power (4 vCPU, 8 GB, 90 GB) komfortabel.

Zwei Dinge solltest du vor der Bestellung wissen: Port 25 ist bei den VPS gesperrt, und ein 1-vCPU-Tarif trägt keine dauerhaft CPU-lastige Arbeit. Zu beidem unten die Details. Dazwischen stehen alle Tarife mit den Preisen der Tarifseite, die Frage KVM oder Container, die Posten, die auf den Monatspreis draufkommen können, und die Punkte, die du vor dem Klick auf „Bestellen“ klären solltest.

> **Kurz entschieden**
> - Website, Bot, Testsystem, kleine Nextcloud: **VPS One, 5 €/Monat** (1 vCPU, 2 GB RAM, 25 GB NVMe)
> - Docker-Stack, kleiner Shop, Nextcloud mit Datenbestand: **VPS Basic, 10 €/Monat** (2 vCPU, 4 GB, 50 GB)
> - Datenbank, mehrere Dienste parallel, modded Minecraft: **VPS Power, 20 €/Monat** (4 vCPU, 8 GB, 90 GB)
>
> 👉 [Alle AVA-Tarife und aktuellen Preise ansehen](https://my.ava.hosting/aff.php?aff=15562)

## Alle Tarife der VPS-Reihe im Vergleich

Die Tarifseite listet sieben Pakete. Alle mit vollem Root-Zugang, Control Panel, wöchentlichem Backup, DDoS-Schutz, 99,9 % SLA und unbegrenztem Traffic.

| Tarif | vCPU | RAM (ECC) | NVMe | Preis | Bestellen |
| --- | --- | --- | --- | --- | --- |
| VPS Nano | 1 | 512 MB | 20 GB | 11 €/Jahr | [VPS Nano](https://my.ava.hosting/aff.php?aff=15562) |
| VPS One | 1 | 2 GB | 25 GB | 5 €/Monat | [VPS One](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Basic | 2 | 4 GB | 50 GB | 10 €/Monat | [VPS Basic](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Lucky | k. A. | k. A. | k. A. | 15 €/Monat | [VPS Lucky](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Power | 4 | 8 GB | 90 GB | 20 €/Monat | [VPS Power](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Extra | 6 | 12 GB | 120 GB | 30 €/Monat | [VPS Extra](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Ultra | 8 | 16 GB | 160 GB | 40 €/Monat | [VPS Ultra](https://my.ava.hosting/aff.php?aff=15562) |

Zwei Zeilen brauchen eine Fußnote. Der VPS Nano wird mit einem Jahrespreis von 11 € ausgewiesen und war beim Abruf der Seite als nicht verfügbar markiert („0 Available“). Beim VPS Lucky nennt die Übersicht nur den Preis von 15 € im Monat, keine Leistungsdaten; die stehen erst auf der Bestellseite.

Der Sprung von einer zur zwei vCPU kostet 5 €, der von zwei zu vier weitere 10 €. Das ist der relevanteste Preisunterschied in der Reihe: Wenn dein Projekt an der CPU hängt, ist der Wechsel von Basic auf Power deutlich wirksamer als jede RAM-Aufrüstung.

### Daneben: die Reihe „Self-hosted Start“

AVA Hosting führt eine zweite, günstigere Paketreihe mit eigenen Namen. Sie beginnt bei 2 € im Monat und ist bei gleichem Preis gleich groß oder größer bemessen als die VPS-Reihe. Die Seite nennt pro Paket nur vier Werte: vCPU, RAM, NVMe und unbegrenzten Transfer. Angaben zu Backup, DDoS-Schutz oder Port-Geschwindigkeit fehlen in dieser Übersicht.

| Tarif | vCPU | RAM | NVMe | Preis | Bestellen |
| --- | --- | --- | --- | --- | --- |
| Start | 1 | 1 GB | 15 GB | 2 €/Monat | [Start](https://my.ava.hosting/aff.php?aff=15562) |
| Mini | 1 | 2 GB | 25 GB | 5 €/Monat | [Mini](https://my.ava.hosting/aff.php?aff=15562) |
| Basic | 2 | 4 GB | 50 GB | 10 €/Monat | [Basic](https://my.ava.hosting/aff.php?aff=15562) |
| Pro | 4 | 8 GB | 100 GB | 20 €/Monat | [Pro](https://my.ava.hosting/aff.php?aff=15562) |
| Business | 6 | 12 GB | 150 GB | 30 €/Monat | [Business](https://my.ava.hosting/aff.php?aff=15562) |
| Power | 8 | 16 GB | 200 GB | 40 €/Monat | [Power](https://my.ava.hosting/aff.php?aff=15562) |

Der 2-€-Tarif ist der eigentliche Einstiegspreis des Anbieters, nicht die 5 € des VPS One. Wer nur einen Bot oder eine statische Seite hostet, kommt damit aus. Vor der Bestellung lohnt eine Frage an den Support, worin sich die beiden Reihen unterscheiden; aus den Tarifseiten geht das nicht hervor, und ein fehlendes Backup wäre ein Ausschlusskriterium.

## KVM statt Container: was das praktisch bedeutet

AVA Hosting virtualisiert die VPS mit KVM. Jede Instanz bekommt eigene virtuelle Hardware und einen eigenen Kernel. Der Anbieter bewirbt die vCPU-Kerne als dediziert zugewiesen, also nicht als überbuchten Pool, aus dem sich Nachbarn bedienen.

Der Kontrast dazu ist LXC, wie es viele sehr billige Einstiegstarife nutzen. Bei LXC teilen sich alle Container den Kernel des Hostsystems, statt jeweils ein komplettes Betriebssystem zu starten. Das spart Overhead und ist der Grund, warum manche Anbieter 1-GB-Container für unter 3 € im Monat verkaufen können. Der Preis dafür sind drei Grenzen: kein eigener Kernel, keine eigenen Kernel-Module, keine verschachtelte Virtualisierung. Für Webserver, Datenbanken, Gameserver, Voiceserver, Bots und Docker-Workloads ist das folgenlos. Wer in seinem Server eine weitere virtuelle Maschine betreiben, einen angepassten Kernel booten oder ein Modul nachladen will, das im Host-Kernel fehlt, braucht KVM.

Bei AVA Hosting fällt die erste Einschränkung damit weg. Was KVM nicht garantiert, ist Rechenzeit: Die Virtualisierungsschicht legt fest, welche Ressourcen eine Instanz sieht, nicht, wie viel CPU-Zeit sie tatsächlich bekommt, wenn der Host ausgelastet ist. Genau darum geht es im Abschnitt zu den Messwerten weiter unten.

👉 [VPS One mit Root-Zugang und KVM ansehen](https://my.ava.hosting/aff.php?aff=15562)

## Was im Preis enthalten ist

Das wöchentliche Backup ist derPosten, der die Rechnung am stärksten verändert. Bei AVA Hosting gehört es bei allen VPS-Tarifen dazu, ebenso der DDoS-Schutz, der Root-Zugang, das Control Panel und 24/7-Support. Bei STRATO ist beim Windows-V-Server ausdrücklich keine Sicherung enthalten; bei IONOS kostet das Acronis-Backup ab 6 Cent pro GB und Monat, für einen 50-GB-Server also rund 3 € monatlich zusätzlich. Über ein Jahr sind das bei AVA 36 €, die du nicht zahlst.

Beim Traffic steht „unbegrenzt“ auf der Seite, mit 1 Gbit/s Portgeschwindigkeit bei allen Tarifen außer dem VPS Nano, der mit 100 Mbit/s läuft. Unbegrenzter Traffic ist in dieser Preisklasse ein Fair-Use-Versprechen, keine garantierte Bandbreite; wer mehrere Terabyte pro Monat ausliefert, sollte das vorher ansprechen.

Zwei Lücken fallen auf:

- **Port 25 ist gesperrt.** Auf der Tarifseite ist das für den VPS Nano ausdrücklich vermerkt. Ein eigener Mailserver, der direkt an fremde MX-Server ausliefert, fällt damit weg. Läuft der Versand über einen SMTP-Relay eines Drittanbieters, ist der geschlossene Port kein Problem.
- **IPv6 wird in der Tarifübersicht nicht genannt.** Wenn du ein eigenes Präfix für Container oder ein /64 für Mail-Reputation brauchst, klär das vor der Bestellung. Bei manitu gehört ein dediziertes /64 zum Standardumfang, bei IONOS ein /80-Netz; bei AVA steht dazu nichts.

👉 [Tarife mit wöchentlichem Backup ansehen](https://my.ava.hosting/aff.php?aff=15562)

## Was zusätzlich kosten kann

Die AVA-Tarifseite nennt keine Einrichtungsgebühr. Ob im Checkout eine anfällt, siehst du erst dort. Zum Vergleich, weil es die Wahrnehmung von „ab 5 €“ verschiebt: STRATO berechnet 9 € Einrichtung pro V-Server, IONOS beim Windows-VPS 10 €.

Drei weitere Posten, die bei anderen Anbietern regelmäßig dazukommen:

- **Zusätzliche IPv4-Adressen**: bei IONOS 5 € pro Monat und Adresse. Wie AVA das handhabt, steht nicht in der Übersicht.
- **Panel-Lizenzen**: eine externe Anbieterübersicht nennt cPanel, Plesk und DirectAdmin als Optionen bei AVA. Ob eine Lizenz im Tarifpreis steckt oder separat abgerechnet wird, geht aus der Tarifseite nicht hervor. IONOS verlangt für Plesk Obsidian 5 € im Monat, und das erst ab dem VPS Linux S mit mindestens 20 GB Speicher.
- **Backup-Speicher**: bei AVA enthalten, bei IONOS und STRATO nicht. Diesen Posten kannst du aus deiner Rechnung streichen.

## Monatspreis, Aktionspreis, Jahrespreis

AVA Hosting weist die Preise als „Starting from“ aus, also als Einstiegspreis der jeweiligen Konfiguration. Der VPS One steht mit 5 € monatlich in der Übersicht, der VPS Nano mit 11 € jährlich. Ein Aktionspreis, der später auf einen höheren Normalpreis springt, ist auf der Tarifseite nicht ausgewiesen.

Bei anderen Anbietern ist genau das die Regel. Eine kleine Übersicht der Einstiegspreise, jeweils ohne Anspruch auf Vollständigkeit der Tarifstruktur:

| Anbieter | Einstieg | Was dahintersteckt |
| --- | --- | --- |
| STRATO Linux VPS | 2 € im ersten Monat, danach 4 € | VPS S mit 1 vCore, 2 GB RAM, 60 GB NVMe; 9 € Einrichtung |
| STRATO Windows VPS | 13 € in der Aktion, danach 20 € | VPS M mit 2 vCores, 4 GB RAM, 120 GB NVMe; Backup nicht enthalten |
| IONOS VPS | ab 2 € laut Seitentitel | verfügbar, aber ohne Tarifbezug; Backup ab 6 Cent/GB/Monat, zusätzliche IPv4 5 €/Monat |
| manitu vServer | ab 2,49 € laut Seitentitel | KVM, /64 IPv6 inklusive, keine Einrichtungsgebühr, Laufzeit 1 Monat |

Die Rechnung für das erste Jahr lautet immer: Aktionspreis + Restmonate × Normalpreis + Einrichtung. Beim STRATO Linux VPS M sind das 3 € + 11 × 10 € + 9 € = 122 €. Beim AVA VPS Basic sind es 12 × 10 € = 120 €, ohne Einrichtung und ohne Sprung. Das ist der eigentliche Vergleich, nicht die Zahl im Werbebanner.

## Ein dokumentierter Fall von CPU-Steal

Im September 2026 veröffentlichte ein Nutzer auf dev.to eine Messung zu einem KVM-VPS von AVA mit einer vCPU. Über eine Minute gemittelt lag der CPU-Steal bei 32,73 %, die Pressure-Stall-Information zeigte knapp 99 % „some“-Druck, die Runnable-Queue erreichte 11 bei einem einzelnen Kern, iowait blieb bei 0 %. Die Kombination aus vollem Steal, null Idle und null iowait spricht für CPU-Konkurrenz auf dem Host und gegen ein Storage-Problem.

AVA bewirbt auf der VPS-Seite dedizierte vCPU-Kerne, deren Leistung von anderen Kunden nicht beeinflusst wird. Diese Messung passt nicht zu der Aussage. Sie belegt allerdings auch keinen Dauerzustand der Plattform: Es ist ein einzelner Server unter einer bestimmten Last, und der Nutzer schreibt das selbst dazu.

Bemerkenswert ist der Ausgang. Der Nutzer kündigte und bekam den Betrag vollständig und ohne Diskussion zurück. Eine externe Bewertungsseite führt daneben eine Kundenstimme mit 4,0 von 5 Punkten, die die Verfügbarkeit als ordentlich, den Support aber als langsam und die Ladezeiten als schwankend beschreibt. Beides sind Einzelstimmen, keine Erhebung.

Für die Tarifwahl folgt daraus eine einfache Regel: Ein 1-vCPU-Tarif ist keine Maschine für dauerhaft CPU-lastige Arbeit. Kompilieren, Transcodieren, eine Spielinstanz mit vielen Chunks oder eine Datenbank mit hoher Last gehören auf mindestens 2, besser 4 vCPU. Beobachte in den ersten Tagen `%steal` in `top` oder `vmstat` und den Druck in `/proc/pressure/cpu`. Dann siehst du an deinem eigenen Server, ob die Zuteilung hält, was sie verspricht.

## Für wen AVA Hosting passt, für wen nicht

Die Server stehen in Moldau. Eine externe Anbieterübersicht beschreibt das Rechenzentrum als gehärtete Anlage in einem ehemaligen Militärbunker bei Chișinău, mit eigener Hardware statt Weiterverkauf. Wer aus rechtlichen oder regulatorischen Gründen einen deutschen Standort mit AV-Vertrag braucht, ist hier falsch; manitu und STRATO bieten das.

Passend ist AVA Hosting für:

- Projekte mit knappem Budget, die KVM, Root-Zugang und ein monatlich abgerechnetes Paket brauchen
- Nutzer, die das wöchentliche Backup als Teil des Preises wollen statt als Zusatzposten
- Bots, Websites, kleine Clouds und Testsysteme, bei denen ein einzelner Kern genügt
- alle, die keine Lust auf Aktionspreise mit Sprung nach drei Monaten haben

Nicht passend:

- eigener Mailserver mit direktem Versand über Port 25
- garantierte CPU-Leistung für Single-Thread-Last
- Projekte, die ein dokumentiertes IPv6-Präfix voraussetzen
- alle, die einen Managed-Service oder eine deutschsprachige Rechtsabteilung als Vertragspartner wollen

## Welcher Tarif für welches Projekt

- **Statische Website, Bot, Uptime-Monitor:** VPS One, 5 €/Monat. Eine vCPU und 2 GB reichen für alles, was keine Datenbank mit Wachstum hat.
- **WordPress mit Cache, Nextcloud für bis zu zehn Nutzer:** VPS Basic, 10 €/Monat. Die zweite vCPU macht sich bemerkbar, sobald PHP und MySQL parallel arbeiten.
- **Docker mit Reverse Proxy, Anwendung und Datenbank:** VPS Power, 20 €/Monat. Drei Container auf einem Kern sind ein Rezept für Wartezeiten.
- **Modded Minecraft mit zehn und mehr Spielern:** VPS Power oder VPS Extra. Chunk-Generierung ist single-thread-lastig und frisst RAM.
- **Mehrere Sites, CI-Runner, Datenbank mit Working-Set:** VPS Extra für 30 € oder VPS Ultra für 40 €.
- **Nur ausprobieren:** die 2-€-Stufe der Self-hosted-Start-Reihe, nachdem du geklärt hast, ob Backup und DDoS-Schutz dazugehören.

Vor dem Bestellen bleiben zwei Punkte zu klären, weil sie nicht in der Tarifübersicht stehen: ob im Checkout eine Einrichtungsgebühr oder ein abweichender Verlängerungspreis auftaucht, und ob IPv6 enthalten ist. Beides lässt sich in zwei Minuten per Ticket fragen und erspart die Überraschung auf der ersten Rechnung.

Für die meisten Leser, die eine Website, einen Bot oder eine kleine Cloud betreiben, ist der VPS One zu 5 € im Monat der richtige Einstieg. Erst wenn Docker mit mehreren Diensten dazukommt, lohnt der Sprung auf 10 oder 20 €.

👉 [VPS One für 5 €/Monat bei AVA Hosting ansehen](https://my.ava.hosting/aff.php?aff=15562)
