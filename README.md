# Minecraft Skript Kolekce

Toto repozitář / složka obsahuje kolekci scriptů pro Minecraft server využívající plugin **[Skript](https://github.com/SkriptLang/Skript)**. Skripty pokrývají širokou škálu herních mechanik, od základních serverových funkcí, přes ekonomiku až po minihry a specifické role-play (RP) činnosti.

## 📂 Struktura složek a skriptů

Kód je rozdělen do několika logických kategorií (složek) podle jejich zaměření:

### 🏙️ Alexandrie (`/alexandrie/`)
Skripty specifické pro lokaci (či město) Alexandrie. Obsahuje lokální mechaniky a aktivity:
- `alexalchymie.sk` - Alchymie a výroba lektvarů.
- `alexdroga.sk`, `alexpivo.sk` - Specifické spotřebitelné předměty a jejich efekty.
- `alexheist.sk` - Vykrádání / Heist mechanika.
- `alexlom.sk` - Těžba a zpracování surovin v lomu.
- Ostatní (`alexgive.sk`, `alexhrnce.sk`, `alexkuze.sk`, `alexlokace.sk`).

### 🎰 Gamba (`/gamba/`)
Široká škála hazardních miniher a mechanik pro kasíno:
- `kasino_base.sk` - Základní systém pro kasíno.
- Minihry: `ruleta.sk`, `plinko.sk`, `automat.sk`, `karty.sk`, `skorapky.sk`, `stiracilosy.sk`, `tower.sk`, `hrobka.sk`, `anubis.sk`.

### 🏡 Město (`/mesto/`)
Produkční systémy, povolání a městské aktivity:
- Zemědělství a pěstování: `farma.sk`, `trava.sk`, `vcelin.sk`, `vino.sk`.
- Ilegální aktivity: `mandroga.sk`, `opium.sk`.
- Další aktivity: `lazne.sk`, `obrana.sk`, `tezba.sk`.

### ⚙️ Server (`/server/`)
Základní technické a administrativní skripty pro chod serveru:
- `autologin.sk` - Systém pro automatické přihlášení (případně napojení na AuthMe).
- `discord.sk` - Propojení s Discordem.
- `role.sk` - Správa rolí/povolání.
- `OMEZENI_POHYBU.sk` - Restrikce pohybu hráčů.
- `anvil_block.sk`, `craftblock.sk` - Omezení specifických bloků nebo craftingu.

### 🌲 Venkov (`/venkov/`)
Profese a aktivity typické pro venkovské oblasti:
- `drevorubec.sk` - Profese dřevorubce.
- `kovarna.sk` - Profese kováře / mechaniky v kovárně.

### 📜 Kořenové skripty (Základ)
Všeobecné herní systémy nezařazené do konkrétních složek:
- `cestovani.sk` - Systém cestování (např. teleporty, doprava).
- `Durabilityminus.sk` - Vlastní mechanika poškozování nástrojů a zbraní.
- `Event.sk` - Systém pro správu serverových eventů.
- `konzumovani.sk` - Úprava konzumace jídla nebo speciálních předmětů.
- Další (`jmenoklik.sk`, `legendary.sk`, `migrace.sk`, `prohledat.sk`).

## 🛠️ Instalace a Použití

1. Ujistěte se, že váš Minecraft server běží na softwaru podporujícím pluginy (Spigot, Paper, Purpur atd.).
2. Stáhněte a nainstalujte plugin **[Skript](https://github.com/SkriptLang/Skript/releases)** kompatibilní s vaší verzí serveru.
3. Zkopírujte všechny `.sk` soubory a složky z tohoto repozitáře do složky `plugins/Skript/scripts/` na vašem serveru.
4. Připojte se na server nebo do konzole a použijte příkaz:
   ```
   /sk reload all
   ```
   *Alternativně můžete načíst konkrétní skript pomocí `/sk reload <nazev_skriptu>`.*

## ⚠️ Závislosti (Addony)
Zkontrolujte kód jednotlivých skriptů. Je pravděpodobné, že některé pokročilé funkce (např. Discord propojení, inventáře, NBT tagy) budou kromě základního pluginu Skript vyžadovat populární addony, jako např.:
- **SkBee** (NBT, recepty, scoreboardy)
- **Vixio** nebo **DiSky** (Propojení s Discordem, využíváno v `discord.sk`)
- **Skript-GUI** / **TuSKe** (Tvorba inventářů a menu)
