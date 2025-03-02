# git-flow-assignment

In dit project wordt git-flow gebruikt om te oefenen met git acties. Het doel hiervan is om te trainen met Git.


## v1.0 release
Hierbij is de eerste versie 1.0 gereleasete.



# Documentatie
Om een beter beeld te geven wat de acties die uitgevoerd zijn voor dit project wordt hieronder beschreven welke specifieke commando's zijn uitgevoerd.

## 1) Repository Opzetten
- Om te beginnen ik heb een nieuwe repository aangemaakt op GitHub. Hierbij heb ik de GUI gebruikt (de browser-versie van GitHub).
- Ik heb deze repository git-flow-assignment genoemd.
- GitHub heeft mij twee opties getoond om het project lokaal te clonen ik heb daar de eerste van uitgekozen en alle commando's die erbij horen uitgevoerd.

// DISCLAIMER: Op verzoek van Raymon wilde ik chronologisch werken. Daarom heb ik niet op tijd gezien dat ik het proces moest documenteren, waardoor ik de
commando's niet heb opgeschreven.

## 2) Eerste Commit
- Ik heb direct een README.md gekregen van GitHub. Daardoor ben ik vergeten om zelf een project omschrijving toe te voegen. Dus bij deze voeg ik het toe.
- Ik heb dus ook de README niet handmatig commit en gepusht naar de main branch.

## 3) Git Flow Instellen
- De git repository heb ik geïnitialiseerd met 'git flow init'
- Dit heeft een serie van vragen getriggerd en ik drukte op enter bij elke vraag om de standaarwaarde te gebruiken. Zo heb ik de branches main, develop en de
benamingen van hotfix, release, etc gekregen.

## 4) Feature Branch
- Nadat de repository toch opgezet was met 'git flow init', heb ik een nieuwe branch aangemaak met 'git checkout -b "feature/add-welcome-message"'
- Omdat ik 'checkout -b' gebruikte ging git meteen naar de branch toe nadat die aangemaakt was, dit in tegenstelling tot een branch aanmaken met 'git branch nieuwe-branch'
en daarna 'git checkout nieuwe-branch'.
- Dan was de bedoeling dat ik daar een nieuwe file zou aanmaken met de welkomstboodschap, dat heb ik gedaan door de GUI van Windows Explorer te gebruiken. In het
bestand heb ik paar zinnen tekst geschreven.
- Daarna heb ik mijn standaard 5 stappen gevolgd
	1) git status
	2) git add .
	3) git commit -m "commit message"
	4) git pull (meestal om de huidige branch te pullen, maar met dit project heb ik deze stap geskipt)
	5) git push
Dit heeft een terugkoppeling van git getriggerd dat deze branch nog niet online staat. Dan heb ik de --set-upstream copy-pastad van de terminal en daardoor kon het wel gepusht worden.
- De Pull Requests heb ik allemaal via de GUI van GitHub gedaan. Waarin ik online kan zien wat de base is en wat de compare branch is.
// Door automatisme heb ik mijn alle eerste PR zelf gemerged, omdat ik zo erg gewend ben. Dus deze werd niet goedgekeurd door mijn collega.

## 5) Release Branch
- Nieuwe release branch aangemaakt met **'git checkout -b "release/v1.0"'**
- In deze nieuwe branch heb ik de README file aangepast met de huidige versie v1.0
- Nog een keer de 5 stappen doorlopen (status, add, commit, pull (geskipt), push)
- Online een PR aangemakt met GitHub GUI webversie
- Deze keer wel mijn collega gevraagd om feedback (approval en commment) om de merge te voltooien

// Door een misverstand (misinterpretatie van de eisen van de opdracht) heb ik ervoor gekozen om het letterlijk te nemen en de branch naar 2 plekken te mergen, waardoor ik 2 PR's had:
de eerste ging naar 'main' en de andere ging naar 'develop'

## 6) Hotfix Branch
- Ik heb dezelfde stappen gevolgd als bij de Release Branch, maar deze keer heb ik de branch alleen gemergd met 'develop' (nadat die goedgekeurd werd door mijn collega).
- Eenmaal de 'develop' geupdatet heb ik een nieuwe PR gedaan van 'develop' naar 'main'

## 7) Tagging
// Dit is een nieuwe onderdeel voor mij waarbij ik veel moeite had. Ik weet nog steeds niet zo goed of het goed is gegaan of niet. Ik heb wel online geoefend met tagging bij speecifieke commits,
maar daar wist ik de commit hash en daarom kon ik de tag meteen koppelen aan de commit. Hier voor deze opdracht heb ik alleen twee nieuwe tags toegevoegd:
- 'git tag v1.0'
- 'git tag v1.0.1'

en daarna heb ik ze gepusht naar de remote:
- 'git push origin --tags


