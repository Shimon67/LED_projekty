# Šimon Langr
# LED PROJEKTY
# OBSAH
Tento projekt se skládá ze tří LED okruhů 
- [LED podsvícení monitoru](#led-podsvícení-monitoru)
- [LED v PC](#led-v-pc)
- [LED za nápisem REDBULL](#led-za-nápisem-redbull)

Další důležité MARKDOWNY
- [Doplnůjící videa](#doplňující-videa)
- [Konečné zapojení/ konečná podoba](#konečné-zapojení-konečná-podoba)
- [Použité nástroje](#použité-nástroje)
- [Literatura](#literatura)
- [Použité součástky](#použité-součástky)
# LED podsvícení monitoru
Tento projekt se zabývá návrhem a realizací adresovatelného LED podsvícení monitoru s využitím LED pásků typu WS2812B / SK6812 a řídicí jednotky s firmwarem WLED. Cílem je vytvořit funkční, bezpečné a estetické ambientní osvětlení, které zlepší komfort při práci i hraní her.

- projekt je zaměřen na praktické využití znalostí z oboru elektrotechniky, zejména:

- práce s nízkým napětím (5 V DC)

- výpočet elektrického příkonu a proudu

- zapojení digitálních LED

- základní konfigurace mikrokontroleru

## Použité komponenty

 ### Řídicí jednotka

- ESP32 WLED Controller (např. Athom / QuinLED ESP32)

- Firmware: WLED (open-source)

- Komunikace: Wi-Fi

### LED pásek

- Typ: WS2812B nebo SK6812

- Napětí: 5 V DC

- Hustota: 30–60 LED / metr

- Použitá délka: cca 1–2 m

### Napájení

- Zdroj: USB / SATA 5 V nebo externí 5 V adaptér

- Proudová rezerva dle počtu LED

### Další materiál

- Propojovací vodiče

- Oboustranná páska / 3M držáky

- Smršťovací bužírka

## Návrh zapojení

- +5 V ze zdroje na LED pásek

- GND zdroje na GND LED pásku a GND ESP32

- Datový vodič (DIN) na GPIO pin ESP32

 ## Výpočet

- 1 LED ≈ 60 mA při plném bílém svitu

- Počet LED: 60

- Výpočet:

I = 60 × 0,06 = 3,6 A

P = U × I = 5 × 3,6 = 18 W

- Použitý zdroj musí mít minimálně 4 A rezervu

## Software (WLED)
### Konfigurace

- Nastavení počtu LED

- Výběr typu LED (WS2812B / SK6812)

- Nastavení jasu a limitu proudu

### Ovládání

- Webové rozhraní

- Mobilní aplikace

- Podpora efektů a barevných scén

## Instalace

LED pásek naistaluji, tak aby směřoval směrem ke zdi, aby mě neoslňoval a dělal scénu v pozadí. Kabely uspořádám, aby nebyly vidět tomu můži použít lepící pásku a kabeláž přilepit k okrajům stojanu na monitoru.

## Závěr
- Projekt není připraven na realizaci z důvodu nedostatku financí na komponenty a čas na jeho uskotečnění, ale do konce školního roku bude. Výsledkem bude plně funkční LED podsvícení monitoru s možností bezdrátového ovládání. Řešení je modulární, energeticky nenáročné a vhodné pro další rozšíření (např. synchronizace s hudbou ).
# LED v PC
## WIP
# LED za nápisem REDBULL
## WIP
# Doplňující videa
## WIP
# Konečné zapojení konečná podoba
## WIP
# Použité součástky
- ESP32 WLED Controller
- USB / SATA 5 V nebo externí 5 V adaptér
- WS2812B nebo SK6812 (rozhodne se u realizace)
# Použité nástroje
- kimi k2 chat (https://kimik2.com/chat)
# Literatura
- WLED app (https://kno.wled.ge/)
- WLED features (https://github.com/wled/WLED?tab=readme-ov-file#%EF%B8%8F-features)
