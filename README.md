# min-side-utkast-topic-iac

Repo med konfigurasjon for hvem som kan produsere og konsumere fra min-side-utkast-topicet.

## utkast på min side
_– en enklere inngang til påbegynte søknader og dokument-innsendinger_ <br>
Utkast er underside av min side (tilgjengelig på `<navurl>/minside/utkast`) der bruker
skal kunne finne søknader og dokument-innsendinger hen har begynt å fylle ut, men ikke sendt inn enda.<br>

### Nice! Hvordan kan mitt team få våre ting på utkast-sida?
Koble på min-side-utkast-topicet og kjør på! <br>
_utkast er i beta og støtter for øyeblikket tre hendelser: created, updated, og deleted_
1. Send en created-melding når en bruker har lagra et utkast
2. Send en updated-melding hvis url-en eller tittelen til utkastet har endret seg. 
3. Send en deleted melding når bruker enten har sendt inn søknaden eller slettet utkastet.
   
Formatet på meldingene er beskrevet i [tms-utkast reopet](https://github.com/navikt/tms-utkast).
Det finnes også et [message-builder bibliotek](https://jitpack.io/#navikt/tms-utkast) som lager meldingene for deg.
NB! Det er kun ting som **ikke er innsendt** som skal ligge på utkast-siden.

## Hvordan kobler jeg meg på min-side-utkast-topic-et?
**For skrivetilgang**

```
- team: myTeam
  application: myApplication
  access: write 
```
**For lesetilgang**

```
- team: myTeam
  application: myApplication
  access: read 
```

          
Når en skal spesifisere topic-navn i sin app må man også ha med navn på namespace der topic ligger.
For alle topicer i dette repoet vil dette være min-side.

For eksempel: min-side.aapen-utkast-v1

## Henvendelser
Spørsmål knyttet til koden eller prosjektet kan rettes mot https://github.com/orgs/navikt/teams/min-side eller 
slackkanalen #brukernotifikasjoner
