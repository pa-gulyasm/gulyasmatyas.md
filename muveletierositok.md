# Műveleti Erősítők (Op-Amp)

## 1. Bevezetés
- A műveleti erősítő (Op-Amp) egy elektronikai eszköz, amelyet analóg jelek erősítésére használnak.
- A leggyakrabban használt műveleti erősítők integrált áramkörök (IC) formájában találhatóak meg.
- Képességei: nagy erősítés, nagyon alacsony torzítás, nagy bemeneti impedancia és alacsony kimeneti impedancia.

## 2. Alapvető jellemzők
- **Bemenet**: Két bemeneti csatlakozó (inverting és non-inverting).
- **Kimenet**: Erősített jel.
- **Működési mód**: A bemeneti feszültségkülönbség alapján működik.
- **Típusok**:
  - **Inverting**: A bemeneti jel a negatív bemenetre kerül.
  - **Non-inverting**: A bemeneti jel a pozitív bemenetre kerül.
<https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTtzrdJXuDpIzWR9Kr18ipIFdFrT9jiX3em5A&s>

## 3. Működési elv
- A műveleti erősítő alapvetően azzal működik, hogy a bemeneti feszültségkülönbséget erősíti.
- **Nyitott hurkú erősítés**: Az erősítő erősítése, ha nincs visszacsatolás (tipikusan több ezer vagy millió).
- **Zárt hurkú erősítés**: Az erősítés a visszacsatolás révén csökkenthető egy kívánt szintre.

## 4. Alkalmazások
- **Jel erősítése**: Analóg jelek erősítése.
- **Szűrők**: Alacsony-, magas- és sávszűrők.
- **Integrálók és differenciálók**: Matematikai műveletek végzése analóg formában.
- **Analóg számítógépek**: Bonyolult számítási műveletek végrehajtása.

## 5. Műveleti erősítők jellemzői
- **Kimeneti feszültség**: A műveleti erősítő kimeneti feszültsége az erősített bemeneti feszültség,
    de a kimeneti feszültség korlátozott a tápegység feszültségszintjeihez.
- **Bemeneti impedancia**: Nagyon magas, így nem terheli a bemeneti jelet.
- **Kimeneti impedancia**: Nagyon alacsony, így könnyen illeszthető más eszközökhöz.

## 6. Példa kapcsolások
### Inverting erősítő
```plaintext
         Rf
Vin ----/\/\----+---- Vout
                |
               GND

          Vin
            |
           R1
            |
            +---- Vout
            |
           R2
            |
           GND
