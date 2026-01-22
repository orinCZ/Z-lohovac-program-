# Zálohovací program (Backup Tool)

![Version](https://img.shields.io/badge/version-3.0.10-blue)

Komplexní nástroj pro automatické zálohování souborů a složek s podporou šifrování, komprese a vzdálené správy.

## 🚀 Hlavní funkce

*   **Chytré zálohování:** Automatická detekce disků (UUID), inkrementální zálohy a kontrola integrity souborů.
*   **Bezpečnost:** Šifrování záloh (AES-256) s možností vázání na konkrétní hardware (HW-tied encryption).
*   **Komprese:** Podpora formátů ZIP, 7z a tar.gz pro úsporu místa.
*   **SMART Monitoring:** Integrovaná diagnostika zdraví disků s historií a grafy. Automatický "Kill-switch" zastaví zálohu při detekci degradace disku.
*   **Vzdálená správa:** Možnost ovládat a konfigurovat zálohování přes síť pomocí aplikace Backup Controller.
*   **Plánovač:** Automatické spouštění záloh v nastavený čas nebo inteligentně podle vytížení CPU.
*   **Gamifikace:** Získávejte "Backup Score" (🏆) za pravidelné a úspěšné zálohování.

## 🛠️ Instalace a spuštění

Aplikace je distribuována jako spustitelný soubor `.exe` pro Windows.

1.  Stáhněte si nejnovější verzi ze sekce Releases.
2.  Spusťte `BackupTool.exe`.
3.  V nastavení zvolte zdrojové složky a cílový disk.

## 📱 Vzdálená správa

Součástí balíku je i **Backup Controller**, který umožňuje:
*   Sledovat průběh zálohy v reálném čase.
*   Spouštět a zastavovat zálohy na dálku.
*   Měnit konfiguraci klienta a spravovat bezpečnostní klíče.
*   Zobrazit reporty a detailní stav disků.

---

*Tento projekt je chráněn autorským právem. © Jakub Kadlec 2026.*