# Voorbereidingsbesluit bij omgevingsverordening NH2022 (Noord-Holland)
## 2021-03-02
- Het besluitgedeelte staat nu in het word-bestand (bewerkt) tussen de titel en de eerste hoofdstukkop. Dit is niet optimaal. Afgesproken is om ook het besluitgedeelte op te nemen in het sjabloon. Hiervoor komt er een opmaakprofiel 'Titel' bij om de titel van besluit en regeling te markeren. De plaats van element 'Conditie' wordt dan ook direct duidelijk, namelijk tussen titel en hoofdstukkop in.
- De transformatie word2imop heeft wat metadata omtrent document en procedure nodig. Hiervoor heb ik ook waarden nodig voor overheidsdomein, onderwerpen, rechtsgebieden. De rest heb ik 'ongeveer' ingevuld.
- Voor alle gemeenten is een WijzigArtikel-WijzigBesluit nodig.
- Is er een intrekkingsartikel nodig?
- Er is een conditie verplicht met daarin een artikel over voorrangsbepalingen.
- Aan artikel X.1 is een geometrie toegekend. Aan de OP-kant moet de vaststelling van een geometrie een noemer 'Noord-Holland' hebben. Deze wordt in de bekendmaking weergegeven als een landingspagina. Een tweede nieuwe methode is via het ambtsgebied. Dan wordt het niet vastgelegd als GIO.
- Aan artikel X.1 hangt een activiteit 'geiten houden'. Hiervoor is een activiteitregelkwalificatie nodig en een activiteitengroep.
- Aan artikel X.1 hangt een gebiedsaanwijzing die verder ingevuld moet worden.
- Aan artikel X.1 hangt een tweede lid '2.' die eigenlijk onderdeel is van het besluit, niet van de regeling.
- Begrip 'Windturbine' zal onderdeel worden van een begrippenlijst in een artikel.
- Is 'Toelichting' bedoeld als motivering?
## 2021-05-11
Voor het voorbereidingsbesluit zijn enkele (open) aandachtspunten:
- Aangeleverd was het grondgebied van Provincie Noord-Holland. Deze is niet gebruikt omdat de regelingen de grondgebieden van de gemeenten Bergen, Schagen en Enkhuizen betreft. Voor het regelingsgebied is het ambtsgebied genomen.
- Aangeleverd was de gml van alle provinciale monumenten in de provincie. Het is niet mogelijk om één gml voor elke tijdelijkRegelingdeel te gebruiken. Dit is omdat de GIO het veld heeftGeboorteregeling heeft dat verwijst naar de afzonderlijke regelingen. De vraag is of voor elk tijdelijkRegelingdeel afzonderlijke gml-en van voorbeschermde provinciale monumenten in de desbetreffende gemeente aangeleverd moeten worden. Nu heeft elk bestand provinciale_monumenten.gml dezelfde poslist, maar een eigen guid.
- In de regelingen worden activiteiten gebruikt. De vraag is welke topactiviteit voor een provinciaal voorbereidingsbesluit gekozen moet worden.
- Voor elke regeling hebben de ow-objecten dezelfde identifier. Voor de provincie is dat ook dezelfde. Bij validatie zal dat problemen geven, omdat dan voor alle andere dan de eerste de foutmelding komt dat het object al bestaat. Hoe gaan we hiermee om?