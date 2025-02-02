## FÖR ATT KÖRA
- Gå till rooten av projektet
- Kör följande komandon: 
- docker-compose down
- docker-compose build --no-cache
- docker-compose up -d
- vänta tills keycloak är helt uppe, kan ta en liten stund extra.

## KEYCLOAK
- logga in poå localhost:8180/admin
- username: admin
- password: password
- Välj customers-realm i menyn uppe till vänster. 
- Välj Users
- Tryck på "Add user"!
- Se till att "email verified" är "ON"
- Välj lämpliga Username, Email etc.
- Tryck spara
- Gå därefter in på fliken "Credentials" och sätt ett lösenord. Det kommer en tooltip där du får skriva in lösenord. Se till att "Temporary" är satt till "Off". Spara lösenordet
- Gå till fliken "Role mapping". Kryssa i "default-roles-customers_realm", och tryck på "Assign role".
- I tooltippen som dyker upp kryssar du i alla roller (för att vara på säkra sidan). Tryck på "Assign".

## WEBB-APPLIKATIONEN
- http://localhost:5173/
- Tryck på "login", och skriv in info som du valde i föregående steg (Keycloak)
- Tyvärr så har jag inte fått applikationen att starta när den körs via Docker. Kör jag backend och frontend var för sig så är det inte några problem.


