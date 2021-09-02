# DT173G, Moment 4
Detta repo innehåller en automatiserad utvecklingsmiljö baserad på Gulp. Projektet är en vidareutveckling av [en föregående uppgift](https://github.com/nlssn/dt173g_m3). Ny funktionalitet har nu lagts till för att kunna använda moderns skriven JavaScript, som ändå är bakåtkompatibel.

För att åstadkomma detta har följande paket lagts till:
- @babel/core
- @babel/preset-env
- gulp-babel

## Installation
För att installera den automatiserade miljön lokalt så använder du följande tre kommandon:

```
git clone https://github.com/nlssn/dt173g_m4.git
cd dt173g_m4/
npm install
```

Vad som sker är att detta git repository klonas till en katalog som heter 'dt173g_m4'. Ifrån den katalogen kan npm installera alla paket genom att läsa igenom filen 'package.json'. 

## Tillgängliga tasks
Standardkommandot ``gulp`` kör alla _tasks_ i en förbestämd ordning för att bygga projektet. När alla filer är klara så börjar BrowserSync att serva dem automatiskt. Därefter håller 'gulp.watch' koll efter eventuella uppdateringar av filer och kör passande _tasks_ vid behov.

Kommandot ``gulp build`` kan användas om du endast vill generera nya filer i '/dist' och inte köra igång den lokala utvecklingsservern.