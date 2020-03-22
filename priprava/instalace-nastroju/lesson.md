Ke tvorbě webů budeme potřebovat několik speciálních programů, které většina profesionálů z praxe používá každý den. Tyto programy pomáhají psát a spravovat kód, komunikovat s počítačem nebo se vyznat v různých verzích vašich rozpracovaných projektů.

## Prohlížeč Chrome

Abychom nemuseli hned zkraje řešit rodíly mezi jednotlivými prohlíženči, budeme všichni svorně používat Google Chrome. Tímto vás rozhodně nenutíme jej používat v soukromí nebo snad psát aplikace pouze pro tento prohlížeč. Krása internetu spočívá právě v tom, že je do velké míry nezávislý na konkrétním softwaru. Pro nás je však ze začátku praktičtější mít vývojová prostředí co nejpodobnější kvůli snadnajšímu řešení problémů, kterých bude i tak dost.

Prohlížeč Google Chrome najdete na jeho oficiálních stránkách https://www.google.com/chrome. Google Chrome je dostupný pro všechny operační systémy.

## Visual Studio Code

Visual Studio Code je textový editor specializovaný na psaní programů a vývoj software. Obsahuje spoustu pomůcek, nástrojů a rozšíření, která zjednodušují programátorům život a umožňují jim spravovat obsáhlé projekty. VS Code je v současné době jedním z nejpoužívanějších programátorských editorů a mnoho profesionálů jej používá při své práci každý den.

Aktuální verzi editoru si naistalujte podle instrukcí na oficiálních stránkách https://code.visualstudio.com. VS Code je dostupný pro všechny operační systémy.

### VS Code - Extensions

VS Code lze přizpůsobit instalací různých rozšíření, které vývojářům poskytují nové možnosti. Rozšíření nainstalujete tak, že kliknete na ikonu rozšíření (Extensions) v levém sloupci na kraji okna VS Code. Případně můžete zmáčknout klávesovou zkratku [[Ctrl]] + [[Shift]] + [[X]]. Pak do okna pro vyhledávání ("Search Extensions in Marketplace") zadáte název příslušného rozšíření.

My Doporučujeme použití následujících rozšíření.

- **Prettier** - Automaticky formátuje váš kód tak, aby vypadal hezky a "profesionálně" 🙂. Budeme jej používat na jazyky jako HTML, CSS, JSON a další.
- **ESLint** - Prettier umí formátovat i JavaScript, ale nedělá to tak hezky jako ESLint, který je zaměřený přímo na JavaScript. ESLint i Prettier bude potřeba ještě nakonfigurovat, což provedeme v následující sekci.
- **Live Server** - Díky tomuto rozšíření nemusíte pokaždé obnovovat stránku, když něco v kódu upravíte. Rozšíření spustí vývojový místní server s funkcí živého opětovného načtení statických a dynamických stránek.
- **Bracket Pair Colorizer** - Díky tomuto rozšířené lépe poznáte, které závorky k sobě patří. Pro nováčky neocenitelná pomoc, pro staré harcovníky možná spíš otrava 🙂.
- **Vetur** - Toto rozšíření nám bude užitečné až začneme pracovat s frameworkem Vue. Můžeme si jej ale nainstalovat už nyní, ať máme všechno hezky pohromadě.

### Nastavení VS Code

Aby se nám s VS Code pracovalo dobře a zároveň nám všem fungovalo stejně, je potřeba vzít následující text a zkopírovat jej do nastavení editoru.

```json
{
  "editor.tabSize": 2,
  "editor.links": false,
  "editor.renderWhitespace": "boundary",
  "editor.insertSpaces": true,
  "editor.wordWrap": "on",
  "files.eol": "\n",
  "editor.minimap.enabled": false,
  "editor.fontSize": 16,
  "eslint.alwaysShowStatus": true,
  "editor.multiCursorModifier": "alt",
  "workbench.colorCustomizations": {
    "editorError.foreground": "#ffff00"
  },
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "prettier.disableLanguages": ["javascript"],
  "window.zoomLevel": 0,
  "eslint.format.enable": true,
  "files.autoSave": "off"
}
```

## NPM a Node.js

Nyní je potřeba nainstalovat balíčkovací systém NPM. Opět následujte instrukce na oficiální stránce https://nodejs.org.

Jakmile máme nainstalován balíčkovací systém NPM, připravíme si složku pro naše projekty. Následující postup zajistí, že ESLint a Prettier budou formátovat všechny naše soubory s kódem podle standardních pravidel.

Někde na svém disku si založte složku s názvem `daweb-projekty`. Ta bude obsahovat většinu vašich projektů a příkladů z této digitální akademie. Do této složky rozbalte všechny soubory obsažené v [tomto ZIP archivu](/czechitas/daweb/assets/priprava/instalace-nastroju/prostredi.zip). Poté se přesuňte do VS Code, otevřete terminál a přesuňte se do této složky. Spustťe následující příkaz.

```shell
$ npm install
```

## Git

Git je verzovací systém, bez kterého se dnes už žádný pořádny programátor neobejde. Najdete jej na adrese https://git-scm.com. Jako všechny zde prezentovaní nástroje, i Git je dostupný pro všechny operační systémy.
