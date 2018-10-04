# Visie en scope

Deze template is gebaseerd op het document `"01 visie en scope(1).pdf"`uit de
voorbeeldcase _Sweet Dreams_ van het vak Software Analysis, aangevuld met
enkele extra rubrieken.

## Visie

### Huidige situatie

De complexiteit is de laatste jaren gestegen door de groei van studenten en bedrijven die interesse hebben in de studenten. Momenteel kunnen bedrijven via een GoogleDoc hun opdracht bekend maken aan PXL-IT, deze wordt dan bekeken door de stagecoördinator en indien goedgekeurd op blackboard geplaatst. Via Blackboard kunnen de studenten dan de potentiële stage opdrachten afgaan en zo hun selectie maken.
Voor het bij de studenten terecht komt moet die stagecoördinator door enkele GoogleDocs gaan, die samen één groot excel vormen, met nog eens extra pdf's waar het nog eens per bedrijf apart in komt te staan, ... Er wordt dus gebruik gemaakt van veel verschillende platformen en soorten documenten wat uiteindelijk voor een slecht overzicht zorgt voor de stagecoördinator.

### Gewenste situatie

De administratie voor de stage op één platform samenbrengen zodat er meer overzicht komt. Voor de bedrijven zou dit bijvoorbeeld zijn dat ze via de webapplicatie hun gegevens ingeven, maar later ook kunnen opvolgen via de webapplicatie als de studenten hun opdracht interessant vinden. Voor studenten creeërt dit ook weer overzicht want het uiteindelijke doel is om ook een soort filter te implementeren zodat de studenten makkelijker door de stageopdrachten kunnen zoeken.
Het uiteindelijke doel is dus om af te stappen van de verschillende platformen en dit samen onder een webapplicatie te gooien, met eventuele extra's.

### Businessrequirements

PXL wil het systeem laten ontwikkelen want:
- Ze willen alle informatie centraal hebben op 1 plek.
- Ze willen dat het beheren van stageplekken eenvoudiger is.

## Belanghebbenden

### Eindgebruikers

**Stagebedrijven**

Het bedrijf kan zich inloggen in het systeem via LinkedIn of mailadres, en kan hierna stagevoorstellen indienen die,
nadat ze goedgekeurd zijn , verschijnen op het systeem en zichtbaar zijn voor studenten.

**Studenten**

Studenten kunnen zich inloggen in het systeem via LinkedIn of mailadres en kunnen hierna de stageplekken die
goedgekeurd zijn door de reviewer bekijken en een stageopdracht kiezen.

**Stagecoördinator**

De stagecoördinator kan zich inloggen in het systeem via LinkedIn of mailadres en kan de opdrachten bekijken, filteren en toewijzen.
De stagecoördinator is ook verantwoordelijk voor het beheer van de stagevoorstellen.

**Lectoren**

Lectoren kunnen zich inloggen in het systeem via LinkedIn of mailadres en kan opdrachten mee beoordelen en selecteren voor welke opdrachten en/of stagebedrijf ze beoordelaar willen zijn.

### Gebruikersomgeving

Het systeem wordt gebruikt door studenten, stagebedrijven, lectoren en de stagecoördinator. Deze kunnen zich inloggen via een web-based
applicatie. Voor de stagecoördinator wordt er een extra desktop client voorzien.

### Overige belanghebbenden

**PXL-promotor**

PXL-promotors worden via het systeem toegewezen aan stagiairs. 

## Systeemscope

### Omschrijving van het systeem

De belangrijkste functionaliteiten van het systeem zijn dat stagebedrijven stagevoorstellen kunnen indienen
die daarna door een reviewer behandeld kunnen worden. Er moet ten alle tijden een goed overzicht zijn van de
status waarin het stagevoorstel zich bevindt (in behandeling, afgewezen, geaccepteerd). Wanneer het stagevoorstel
goedgekeurd is door de reviewer wordt er een uitnodiging verzonden naar het stagebedrijf voor het handshake event.
Studenten kunnen, zodra de stagevoorstellen goedgekeurd zijn, verschillende voorstellen bekijken en deze eventueel selecteren als stageopdracht.
Hierna stelt de stagecoördinator de stagecontracten op en worden deze mogelijk digitaal ondertekend.
Dit zijn tegelijk ook de minimum vereisten.

Verder zal het mogelijk zijn voor de studenten de voorstellen te filteren op basis van hun voorkeur. 
Voor bedrijven zal bij hun opdrachten zichtbaar zijn hoe vaak deze bekeken is, maar niet door wie.
Lectoren krijgen de mogelijkheid om bepaalde voorstellen of bedrijven te selecteren waar ze beoordelaar van de opdracht willen zijn, en hun mening geven over de opdracht.
De stagecoördinator kan via de desktop versie de gegevens van bedrijven zoals adres, telefoonnummer, ... bijhouden en de stagevoorstellen beheren. Het zal mogelijk zijn om er statistieken van te maken en de stagevoorstellen te archiveren.

### Positionering van het systeem

Het systeem zal draaien op een Azure server van Microsoft, die gratis ter beschikking gesteld is aan studenten.
Voor het digitaal ondertekenen maken we gebruik van de software van Belgium eID.
Ook maken we gebruik van een Oracle database.

### Globale gebruikersrequirements

Bij de volgende werkzaamheden is geautomatiseerde ondersteuning van het systeem gewenst:
- het stagebedrijf wil een stagevoorstel indienen of aanpassen.
- het stagebedrijf en de student willen de stagedocumenten digitaal ondertekenen.
- de student kan de stages bekijken.
- de student kan een stagevoorstel selecteren.
- de student en stagecoördinator kunnen filteren op bepaalde critia.
- de PXL-IT lector kan de stagevoorstellen bekijken en goedkeuren.
- de PXL-IT lector kan een voorkeur opgeven voor de begeleiding van een stage.
- de stagecoördinator kan permissions uitdelen.
- de stagecoördinator kan het stagedocument opstellen.
- de stagecoördinator kan de gegevens van de stagebedrijven exporteren.
- de stagecoördinator kan het aantal studenten controleren per stagebedrijf.
- de stagecoördinator kan statistieken trekken uit de gegevens.
- de stagecoördinator kan bevragingen versturen.
- de stagecoördinator kan een PXL-promotor toekennen.
- De stagecoördinator wilt de goedgekeurde opdrachten beschikbaar stellen. 
- De stagecoördinator kan opdrachten afkeuren.
- Lectoren kunnen bepaalde stageopdrachten beoordelen.
- Lectoren kunnen online aanduiden voor welke stageopdracht ze begeleider willen zijn.
- De stagecoördinator kan bedrijven uitnodigen voor het handshake event.

### Niet-functionele requirements

Het systeem moet aan volgende kwaliteitseisen voldoen:
- het systeem moet juist aangeven als een stagevoorstel al gekozen is of niet.
- het systeem moet goed functioneren met de software van Belgium eID.
- de desktop versie van het systeem moet goed kunnen functioneren met de web-based versie van het systeem.
- het systeem moet aangeven hoe vaak een opdracht bekeken is.

## Voorlopige planning

### Risico's

- Eerste ervaring met web-based applicatie.
- Werken in team kan niet altijd even goed verlopen.
- Onvoldoende kennis over bepaalde onderdelen.
- Missen van deadlines door tijd verkeerd in te schatten.
- Bepaalde zaken toch niet kunnen realiseren met huidig niveau.
- ...

### Huidig kennisniveau

- OO - principe
- ADO.Net
- Entity framework
- nUnit testen
- ...

We beschikken over een redelijk niveau waarbij we op vlak van coderen en logica niet al te veel problemen zullen hebben.

### Plan van aanpak

We gaan beginnen met het project uit te stippelen waar we naar toe willen, dit vooral met de scope en het SUC schema. Hierna verdelen we de taken naar de programmeersterktes van elk teamlid, gepaard met iets waar ze nog geen ervaring mee hebben. Dit om een persoonlijke baat qua kennis te krijgen ook in het project.

We zullen eerst het werk verdelen in delen die 2 a 3 weken vragen. Tijdens zo een sprint verdelen we onderling nog eens het werk. 


De prioriteit van het project ligt in het vervolledigen van de minimumrequirements. Zodra deze compleet zijn, breiden we de applicatie verder uit met mogelijke wensen van de klant.


### Bronnen

- http://stackoverflow.com/
- https://www.pluralsight.com/
- https://www.youtube.com/
- https://www.caveofprogramming.com/
- https://www.codeschool.com/
