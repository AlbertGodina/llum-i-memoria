# Sessió 2: Planificació i anàlisi del cicle de vida

!!! abstract "Dades de la sessió"
    **Durada:** 55 minuts · **Agrupament:** parelles fixes

    **Objectiu:** dibuixar l'esquema elèctric del producte, analitzar-ne l'impacte ambiental i crear el cronograma de treball de les properes 10 sessions.

## Abans de tocar cap eina

A la sessió 1 heu triat la imatge i heu generat la litofania. Ara toca pensar: com il·luminarem la peça, quin impacte tindrà el nostre producte i com ens repartirem la feina durant les properes setmanes. Una bona planificació ara us estalviarà temps més endavant.

## Les quatre activitats

| Bloc | Què fem | Temps | Com |
|---|---|---|---|
| 1 | Repàs d'electrònica i càlcul de la resistència | 10 min | Parelles |
| 2 | Anàlisi del cicle de vida del producte | 20 min | Parelles |
| 3 | Rols i cronograma del projecte | 20 min | Parelles |
| 4 | Tancament i verificació | 5 min | Individual |

## 1. Repàs d'electrònica i càlcul de la resistència (10 min)

**Parelles.** Ja sabeu muntar un circuit bàsic amb **font + resistència + LED**. El nostre producte s'il·luminarà amb una **tira LED de 5 V**, així que primer repassem el que ja sabeu i després ho adaptem al producte.

1. Calculeu aproximadament la **resistència** que necessitaria **un sol LED blanc** estàndard alimentat per USB, amb aquestes dades:

    | Dada | Valor |
    |---|---|
    | Tensió de la font (USB) | 5 V |
    | Tensió del LED blanc | 3,0 a 3,2 V |
    | Corrent del LED blanc | 20 mA = 0,020 A |

    La fórmula és: **R = (V font − V LED) / I LED**

2. Dibuixeu l'**esquema elèctric** de la vostra litofania: una **font USB de 5 V**, un **interruptor** (opcional) i la **tira LED**.

!!! tip "Si us costa el càlcul"
    No cal fer cap càlcul complex: el corrent de 20 mA és el valor habitual per a un LED blanc. Podeu fer servir una calculadora en línia o la [calculadora de resistència](../recursos/calculadora-resistencia.md) del web.

??? tip "Pista: comproveu el vostre resultat"
    Amb 3,2 V al LED: (5 − 3,2) / 0,020 = **90 Ω**. Com que 90 Ω no és un valor comercial, a la pràctica es fa servir el valor comercial **immediatament superior** (100 Ω). Així el LED no es crema.

!!! info "Per què la tira LED no necessita resistència?"
    Una tira LED és com molts LED petits, cadascun amb la seva pròpia resistència ja soldada, connectats en paral·lel. Per això es pot connectar directament als 5 V del USB. Si connecteu un LED **sol** directament a 5 V, es crema.

**Producte:** un **esquema elèctric preliminar** (a mà o digital), amb símbols estàndard, i el **càlcul de la resistència** d'un LED.

## 2. Anàlisi del cicle de vida del producte (20 min)

**Parelles.** Cada producte té un cicle de vida: s'origina, s'utilitza i, un dia, s'acaba. Cada fase té un impacte ambiental. Repartiu-vos la feina: una persona investiga el **PLA**, i l'altra, els **components electrònics reciclats** disponibles a casa o a l'escola.

Ompliu la taula del cicle de vida (teniu la plantilla a [Plantilles](../recursos/plantilles.md)) amb **paraules clau o frases curtes**. No cal escriure textos llargs.

| Fase | Preguntes per ajudar-vos | Impacte que identifiqueu |
|---|---|---|
| **Extracció i producció** | D'on ve el PLA? És biodegradable? Quins residus genera la impressora? | |
| **Ús** | Quant consumeix la tira LED? Com afecta la factura de la llum de qui l'utilitzi? | |
| **Fi de vida** | Què passa amb la litofania quan es trenca? Es pot reciclar el plàstic? I els components electrònics? | |

??? tip "Pista per a la fase d'ús"
    La potència que consumeix la tira es calcula amb **P = V · I**. A la sessió 7 en sabreu el valor exacte; ara en podeu fer una estimació: amb 5 V i uns 100 mA, surt **0,5 W**. Compareu-ho amb el consum d'altres aparells de casa vostra: mireu una factura de la llum o l'etiqueta d'un electrodomèstic.

### Dues accions concretes

Quan tingueu la taula, decidiu **dues accions concretes** que farem nosaltres per minimitzar l'impacte negatiu. Per exemple:

- fer servir PLA sobrant;
- reciclar cables USB vells;
- optimitzar els paràmetres d'impressió per estalviar material.

**Producte:** la **taula del cicle de vida** completada i **2 accions de sostenibilitat** identificades.

## 3. Rols i cronograma del projecte (20 min)

**Parelles.**

### Assigneu els rols inicials

A la pàgina [Com treballem](../com-treballem.md) hi ha els quatre rols del projecte. Com que sou dues persones i hi ha quatre rols, **cadascú en porta dos**. Decidiu ara qui lidera quina fase.

| Rol | Responsable de |
|---|---|
| **Dissenyador/a principal** | Tinkercad i mesures precises |
| **Enginyer/a de fabricació** | Bambu Studio i fitxers d'impressió |
| **Tècnic/a electrònic** | Circuit, connexions i seguretat |
| **Documentant/Comunicador/a** | Fotos, captures i preparació del pitch |

Els rols **rotaran** durant el projecte, però ara heu de tenir clar qui fa què. Tots dos participeu en tot, però a cada fase hi ha una persona responsable.

### Feu el cronograma de la parella

Consulteu el calendari de les 12 sessions del projecte i completeu el cronograma amb aquestes fites (també és a [Plantilles](../recursos/plantilles.md)):

| Sessió | Què hem de tenir fet | Responsable |
|---|---|---|
| 3 | Exercicis 1 a 5 de Tinkercad | |
| 4 | Exercicis 6 i 7, i litofania importada i mesurada | |
| 5 | Capsa dissenyada | |
| 6 | Projectes de laminació preparats i enviats a la cua d'impressió | |
| 7 | Circuit LED muntat i funcionant fora de la capsa | |
| 8 | Peces revisades i prototip muntat | |
| 9 | Portafoli digital i guió del pitch | |
| 10 | Acabats i assaig del pitch | |
| 11 | Presentació final | |
| 12 | Lliurament i tancament | |

A més, **marqueu en quin dia espereu tenir la peça impresa i el circuit muntat**. Podeu fer-ho amb la plantilla visual de calendari de la carpeta del projecte: arrossegueu els blocs de temps.

!!! info "Les impressions triguen"
    Imprimir una litofania a 0,1 mm d'alçada de capa és lent. Per això, mentre una peça s'imprimeix, avançareu amb el circuit o amb la documentació.

**Producte:** el **cronograma de la parella**, signat per les dues persones, i els **rols inicials** ben definits.

## 4. Tancament i verificació (5 min)

**Individual.** Marqueu amb ✅ o ❌ cada punt:

- [ ] Hem triat una imatge i l'hem validada a itslitho.
- [ ] Tenim l'esquema elèctric preliminar.
- [ ] Hem completat l'anàlisi del cicle de vida.
- [ ] Tenim el cronograma i els rols definits.

Pugeu tots els productes digitals (captura d'itslitho, esquema, taula del cicle de vida i cronograma) a la **carpeta de Google Drive de la parella**. Reviseu que estigui ordenada.

**Producte:** una carpeta digital ordenada i verificada.

!!! tip "Si us encalleu"
    La taula té caselles per omplir amb paraules clau, no cal fer redaccions. Si no sabeu per on començar l'esquema, repasseu el circuit que ja heu muntat altres vegades: font, resistència i LED en sèrie. Podeu demanar ajuda al docent o a una parella mentor.

**Següent:** [Sessió 3. Introducció al disseny 3D](../fase2-aprenem/s03-tinkercad-basic.md)
