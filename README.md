# Zálohovací program (Backup Tool)

![Version](https://img.shields.io/badge/version-3.1.3-blue)

Komplexní nástroj pro automatické zálohování souborů a složek s podporou šifrování, komprese a vzdálené správy.

## 🔥 Novinky ve verzi 3.0.18
*   **Jednorázová záloha:** Nový režim pro rychlé zálohování bez ovlivnění hlavní konfigurace.
*   **Uživatelské profily:** Možnost přepínat rozhraní mezi režimy Základní, Pokročilý a Expertní.
*   **Vzdálený Restart:** Možnost provést tvrdý restart vzdáleného počítače přes Controller.
*   **Wake on LAN:** Funkce pro probuzení počítačů v síti (včetně hromadného spuštění).
*   **Integrovaná nápověda:** Tlačítko `?` pro zobrazení manuálu (online i offline).
*   **Vylepšené reporty:** Přidán kompletní výpis nastavení do HTML reportu.
*   **2FA Autentizace:** Podpora TOTP pro bezpečný vzdálený přístup.
*   **Auditní logy:** Záznam bezpečnostních událostí do `audit.log`.
*   **Safe Mode:** Fronta akcí pro dočasně nedostupná zařízení.
*   **S3 Cloud:** Nativní podpora pro AWS S3 a kompatibilní úložiště.
*   **VSS Snapshots:** Zálohování otevřených a uzamčených souborů (Windows).
*   **Pokročilé režimy:** Podpora pro Diferenciální a Inkrementální zálohy.
*   **Verifikace:** Kontrola integrity dat po přenosu.

## 🔥 Novinky ve verzi 3.0.14
*   **Debug Console:** Nové okno v Controlleru pro sledování logů v reálném čase (lokální i vzdálené).
*   **Diagnostika sítě:** Přidán nástroj pro testování rychlosti (Speed Test), Ping a Tracert přímo v aplikaci.
*   **Vylepšený SMART:** Detailní zobrazení stavu disků a moderní HTML report.
*   **Indikace chyb:** Oranžové podbarvení zařízení v seznamu při chybě.
*   **Opravy:** Vyřešeny problémy s kolizí portů a stabilitou připojení.

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

Součástí balíku je i **Backup Controller** (Desktop a Android), který umožňuje:
*   Sledovat průběh zálohy v reálném čase.
*   Spouštět a zastavovat zálohy na dálku.
*   Měnit konfiguraci klienta a spravovat bezpečnostní klíče.
*   Zobrazit reporty a detailní stav disků.

### Android Controller
Nová mobilní aplikace (`backup_controller_android.py`) postavená na frameworku Kivy.

*   **Skenování sítě:** Automaticky najde běžící instance Backup Tool v síti.
*   **Git Bus:** Umožňuje ovládání zařízení i bez přímé IP viditelnosti (přes GitHub repozitář).
*   **Sestavení:** Pro vygenerování `.apk` souboru použijte přiložený skript `package_android_controller.sh` (vyžaduje Linux a Buildozer).

---

*Tento projekt je chráněn autorským právem. © Jakub Kadlec 2026.*