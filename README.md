# Elektronska kontrola u savremenom automobilu

## Pregled

Ovaj projekat predstavlja idejnu realizaciju sistema elektronske kontrole u modernom automobilu, zasnovanog na sistemu mikrokontrolera. Svaki mikrokontroler upravlja određenim segmentom automobila, dok centralni računar upravlja svim aktivnostima i prikuplja podatke. Komunikacija između mikrokontrolera se obavlja preko zajedničke asinhrone poludupleks magistrale sa diferencijalnim prenosom signala.

## Podsistemi

1. **Kontrola otvaranja/zatvaranja prozora i otključavanja/zaključavanja**

2. **Kontrola svetla**

3. **Kontrola temperature**

4. **Zadnji parking senzori**

5. **Kontrola ulaska u automobil (RFID)**

6. **Sistem protiv blokiranja točkova (ABS)**

## Projektni zadaci

1. Nacrtati blok šemu sistema.
2. Napraviti projektne zahteve za centralni računar (prihvatanje tastera, prikaz na instrument tabli).
3. Nacrtati projekat hardvera svakog pojedinačnog objekata upravljanja.
4. Definisati formate i protokole rada za poruke koje se prenose po magistralama.
5. Opisati programske poslove mikrokontrolera.
6. Definisati zahteve za odgovarajućim mikrokontrolerom (broj portova, periferije itd.).

## Šeme sistema

- **`block_scheme.drawio`**: Blok šema sistema.
- **`hardware_addr.drawio`**: Hardversko zadavanje adrese mikrokontrolera.
- **`hardware_debounce.drawio`**: Hardversko debaunsiranje tastera i prekidača.
- **`interrupt.drawio`**: Povezivanje podsistema na zajedničku liniju za prekid.
- **`master_<system>.drawio`**: Povezivanje potrebnog hardvera na centralni računar za kontrolu određenog podsistema.
- **`slave_<system>.drawio`**: Povezivanje potrebnog hardvera na mikrokontroler određenog podsistema.
- **`uart.drawio`**: Povezivanje centralnog računara i podsistema preko asihrone poludupleks magistrale sa diferencijalnim prenosom signala (UART).