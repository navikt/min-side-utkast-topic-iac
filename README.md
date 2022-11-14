# min-side-utkast-topic-iac

Repo med konfigurasjon for hvem som kan produsere og konsumere fra min-side-utkast-topicet.

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