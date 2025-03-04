# Feszültségkövető Mérése Oszcilloszkóppal és Függvénygenerátorral

## 1. Célkitűzés
A cél egy feszültségkövető (buffer) áramkör működésének vizsgálata oszcilloszkóppal és függvénygenerátorral.  
A feszültségkövető egy egységnyi erősítésű erősítő, amely biztosítja a nagy bemeneti impedanciát és az alacsony kimeneti impedanciát.

## 2. Szükséges Eszközök
- **Függvénygenerátor** (szinusz, négyszög, háromszög jelek előállítására)
- **Oszcilloszkóp** (bemeneti és kimeneti jelek vizsgálatához)
- **Operációs erősítő** (pl. TL081, LM741, NE5532 stb.)
- **Tápfeszültség** (+Vcc, -Vcc, pl. ±12V)
- **Próbaáramkör (breadboard) vagy forrasztott áramkör**
- **Mérővezetékek és csatlakozók**

## 3. Kapcsolási Rajz
árleszállítás

Másolás

Szerkesztés
   +Vcc
    │
    │
    ├─────────
    │        │
    │        │
┌────

makefile

Másolás

Szerkesztés

**Megjegyzés:**  
- Az **A pont** az operációs erősítő neminvertáló bemenete.
- A kimeneti feszültség (Vout) ideálisan megegyezik a bemeneti feszültséggel (Vin), azaz **Vout ≈ Vin**.

## 4. Mérés Beállítása
1. **Kapcsolás összeállítása** a fent látható rajz alapján.
2. **Függvénygenerátor beállítása**:
   - Frekvencia: **1 kHz**
   - Kimeneti feszültség: **2 Vpp**
   - Jelalak: **szinuszjel**
3. **Oszcilloszkóp csatlakoztatása**:
   - CH1: bemeneti jel (Vin)
   - CH2: kimeneti jel (Vout)
4. **Mérés elvégzése**:
   - Figyeljük meg az oszcilloszkópon, hogy a kimeneti jel követi-e a bemenetet.
   - Vizsgáljuk meg az esetleges fáziseltolódást.
   - Ellenőrizzük, hogy a kimeneti amplitúdó megegyezik-e a bemeneti amplitúdóval.

## 5. Mérési Képletek

A feszültségkövető ideális esetben egységnyi erősítéssel rendelkezik:

\[
A_u = \frac{V_{out}}{V_{in}} = 1
\]

A valós erősítés mérésére használható képlet:

\[
A_u = 20 \log \left( \frac{V_{out}}{V_{in}} \right) \text{ dB}
\]

Ha frekvenciafüggő mérést végzünk, a sávszélességet az alábbi módon határozhatjuk meg:

\[
A_{u(dB)} = 20 \log \left( \frac{V_{out}}{V_{in}} \right)
\]

ahol **A_{u(dB)}** az erősítés decibelben kifejezve.

## 6. Mérési Eredmények
Az alábbi kép mutatja az oszcilloszkóp és függvénygenerátor beállításait a mérés során:

![Feszültségkövető mérés](./0d05075e-9226-42bf-967f-36628d4cd2ba.jfif)

A képen látható:
- A függvénygenerátor kimeneti beállítása: **1 kHz, 2 Vpp szinuszjel**.
- Az oszcilloszkóp által mért bemeneti és kimeneti jelek, amelyek szinte teljesen fedik egymást, igazolva a feszültségkövető működését.

## 7. Következtetés
A feszültségkövető sikeresen követi a bemeneti jelet, ahogy az oszcilloszkópon is látható. Ideális esetben nincs erősítés vagy fáziseltolás, de magasabb frekvenciákon az operációs erősítő paramétereitől függően minimális torzulás előfordulhat.  
A mérési eredmények alapján a feszültségkövető megfelelően működik.

---
**Készítette:** Gulyás Mátyás  
**Dátum:** 2025.02.04.
