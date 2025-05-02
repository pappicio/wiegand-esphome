progetto esphome per tastiere con impronte e rfid. tag e password, per apertura cancello/portone, il tutto con protocollo wiegand.
ho usato: esp8266, poi un esp32 c3 super mini, al momento monto un esp32 s2 mini
tastiera wiegand (ce ne sono milioni online ma uso questa) bluetooth ma con hub wifi va anche in wifi, ma nn serve in realta, basta il br, visto che poi gestisco tutto da codice esphome e volendo da homeassistant per automazioni


la tastiera che ho su è questa: 

https://it.aliexpress.com/item/1005007498553229.html?spm=a2g0o.order_list.order_list_main.123.1efe3696qhH1F7&gatewayAdapt=glo2ita


esp32 s2 mini: 

https://it.aliexpress.com/item/1005006217896066.html


ovviamente gia basta e avanza (nel codice esphome trovate anche ovviamente i pin scelti)


ho aggiunto un tamper con l'ausio di uno switch a leva: 

https://it.aliexpress.com/item/1005008233825861.html


e per evitare (successivamente pero' anche senza, i pin esp32 supportano i 5v, ma se si puo, meglio essere precisi) uno shifter 4 canali da 5v a 3.3, ne ho utilizzati, ovviamente solo 2 dei 4 canali per i 2 fili wiegand (D0 e D1)

https://it.aliexpress.com/item/32612366630.html (questo è gia a 2 canali, ottimo, ma ne aveco qualcuno a 4, riciclo!!!)


ecco tutto, la tastiera funziona una favola e fa il suo, memorizzo su codice le impronte/badge/password permamenti cosi da gestirle a prescindere di homeassistant, ed ho aggiunto un UPS da 1000 VA cosi anche senza rete elettrica, apro quando voglio!
