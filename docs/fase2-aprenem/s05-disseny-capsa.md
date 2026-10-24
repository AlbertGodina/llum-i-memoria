# Sessió 5: Disseny de la capsa funcional

!!! abstract "Dades de la sessió"
    **Durada:** 55 minuts · **Agrupament:** parelles, amb rols (una persona fa el cos i l'altra la tapa)

    **Objectiu:** dissenyar la capsa que allotjarà la litofania i el circuit, garantint que les peces encaixin i que el producte funcioni.

## Una capsa feta a mida

La capsa es dissenya **a partir de les mesures de la litofania** que vau anotar a la [sessió 4](s04-forats-importacio-litofania.md). Això us dona llibertat total de disseny, però té un risc: **un cop impresa, és molt difícil corregir errors** (per exemple, aprimar una paret). Per això avui val la pena revisar bé cada mida abans de passar a imprimir.

## Les tres activitats

| Bloc | Què fem | Temps | Com |
|---|---|---|---|
| 1 | Definim les dimensions i l'estructura | 10 min | Parelles |
| 2 | Modelem la capsa a Tinkercad | 35 min | Parelles, amb rols |
| 3 | Revisió de qualitat | 10 min | Parelles i mentor |

## 1. Definim les dimensions i l'estructura (10 min)

**Parelles.** Farem una **caixa tancada amb tapa**, que protegeix l'electrònica. Tindrà dues parts:

- **El cos:** la caixa, amb una **finestra** al davant, un **encaix** on s'asseu la litofania i una **cavitat** per al circuit.
- **La tapa:** tanca la caixa pel darrere i té el **forat del cable USB**.

De davant cap enrere, el cos té aquesta estructura:

| Zona | Què és |
|---|---|
| Paret del davant (2 mm) | El marc, amb la finestra per on es veu la imatge |
| Encaix (gruix de la litofania + 1 mm) | L'espai on s'asseu la litofania |
| Cavitat (25 mm) | L'espai per a la tira LED, l'interruptor i els cables |
| Darrere | Obert: es tanca amb la tapa |

### Calculeu les dimensions

Agafeu les mesures de la litofania de la sessió 4 i ompliu la columna «La nostra». L'exemple és per a una litofania de 80 × 60 mm i 3 mm de gruix.

| Mida | Com es calcula | Exemple | La nostra |
|---|---|---|---|
| Amplada exterior | amplada litofania + 8 | 88 mm | |
| Alçada exterior | alçada litofania + 8 | 68 mm | |
| Fondària exterior | 2 + (gruix + 1) + 25 | 31 mm | |
| Cavitat (amplada × alçada × fondària) | (amplada + 4) × (alçada + 4) × 25 | 84 × 64 × 25 mm | |
| Encaix (amplada × alçada × fondària) | (amplada + 1) × (alçada + 1) × (gruix + 1 + 25) | 81 × 61 × 29 mm | |
| Finestra (amplada × alçada × fondària) | (amplada − 8) × (alçada − 8) × 3 | 72 × 52 × 3 mm | |
| Tac de la tapa | cavitat − 0,8 a l'amplada i a l'alçada | 83,2 × 63,2 mm | |

!!! info "Per què tantes folgances?"
    Les impressores 3D no són perfectes. Si l'encaix és exacte, la peça no hi entra. Per això l'encaix té **1 mm de joc**, la cavitat deixa **2 mm** a cada costat i la tapa té **0,4 mm** de joc per costat.

!!! warning "Parets de 2 mm com a mínim"
    Cap paret de la capsa no pot ser més prima de 2 mm, o es trencarà en imprimir-la.

**Producte:** un **esbós** (a mà o digital) de la capsa amb les dimensions exteriors i interiors.

## 2. Modelem la capsa a Tinkercad (35 min)

**Parelles, amb rols.** Una persona fa el **cos** i l'altra la **tapa**. Treballeu al disseny `Projecte_Litofania_Final`, on ja teniu la litofania importada.

!!! tip "Per orientar-vos"
    Mireu la caixa amb la **vista frontal** (el cub de la vista, a dalt a l'esquerra). Fixeu-vos que l'**amplada** és d'esquerra a dreta, la **fondària** és de davant cap enrere i l'**alçada** és la vertical. Si no esteu segurs de quin quadre de mida és quin, comproveu-ho mirant com canvia la forma.

### Persona A: el cos (≈ 25 min)

1. **Caixa exterior.** Afegiu un cub amb les mides exteriors: amplada × fondària × alçada (a l'exemple, 88 × 31 × 68).
2. **Cavitat.** Afegiu un altre cub, convertiu-lo en **forat** (*Hole*) i poseu-li les mides de la cavitat (84 × 25 × 64). Alineeu-lo amb la caixa:
    - pel **centre** a l'amplada i a l'alçada;
    - pel **darrere** a la fondària.
3. **Encaix de la litofania.** Afegiu un altre cub-forat amb les mides de l'encaix (81 × 29 × 61) i alineeu-lo igual que la cavitat. Així l'encaix queda just darrere de la paret del davant i s'obre cap a la cavitat.
4. **Finestra.** Afegiu un cub-forat amb les mides de la finestra (72 × 3 × 52). Alineeu-lo pel **centre** a l'amplada i a l'alçada, i pel **davant** a la fondària.
5. **Agrupeu** la caixa i els tres forats. Comproveu-ho: des del davant heu de veure la finestra, i des del darrere, la cavitat oberta.

??? tip "Pista: si queda una capa fina al darrere"
    Si en agrupar veieu una pell fina de plàstic al darrere, feu els forats una mica més llargs i alineeu-los de nou pel darrere.

### Persona B: la tapa (≈ 20 min)

1. **Placa.** Afegiu un cub amb les mides exteriors de la caixa en amplada i alçada, i 2 mm de fondària (88 × 2 × 68).
2. **Tac d'encaix.** Afegiu un altre cub amb les mides del tac (83,2 × 7 × 63,2). Alineeu-lo pel centre a l'amplada i a l'alçada, i pel **davant** a la fondària. Així sobresurt 5 mm per darrere de la placa, i aquesta part és la que entra a la cavitat.
3. **Forat del cable.** Afegiu un cilindre-forat de **5 mm de diàmetre**, gireu-lo 90° perquè travessi la tapa i alineeu-lo pel centre a l'amplada. Pugeu-lo uns **8 mm** amb la fletxa negra, perquè quedi a la part de baix de la tapa.
4. **Agrupeu** la placa, el tac i el forat. Feu servir un color diferent del cos.

Quan acabeu, ajudeu la vostra parella.

### Verificació virtual (≈ 10 min, tots dos)

!!! warning "No agrupeu la litofania amb la capsa"
    La litofania és una peça **separada**: s'imprimirà a part i s'inserirà a la capsa.

1. Poseu la **litofania** dreta (vertical) i col·loqueu-la dins l'encaix.
2. Mireu-la des del davant: la finestra ha de deixar veure la imatge i el marc l'ha de cobrir per les vores.
3. Gireu la vista i comproveu que **no hi ha col·lisions**: cap part de la litofania ha d'entrar en el plàstic de la capsa.
4. Mireu la **tapa** al costat del cos: el tac ha de poder entrar a la cavitat.

!!! tip "Si us bloqueu"
    Podeu començar d'una **capsa de rescat**: un model ja iniciat que només heu d'adaptar a les vostres mesures. La trobareu a [Tinkercad de rescat](../recursos/tinkercad-rescat.md), o la podeu demanar al docent. També podeu consultar la [guia ràpida](../practica-tinkercad/guia-rapida.md).

**Producte:** el disseny complet de la capsa (cos i tapa) a Tinkercad, llest per exportar.

## 3. Revisió de qualitat (10 min)

**Parelles, i després mentor** (el docent o una parella que hagi acabat abans).

Mostreu el vostre disseny i responeu aquestes preguntes de control:

- [ ] Hi ha **prou marge** per als components electrònics (tira LED, interruptor, cables)?
- [ ] El **forat del cable** és accessible?
- [ ] La **tapa** es pot obrir i tancar virtualment?
- [ ] La **litofania** hi cap i la finestra en mostra la imatge?
- [ ] Cap paret no és més prima de **2 mm**?

**Producte:** l'**aprovació tècnica** del disseny abans de passar a la laminació.

## Abans de marxar

- [ ] Tenim el cos i la tapa dissenyats.
- [ ] Hem comprovat la litofania dins l'encaix.
- [ ] El docent o una parella mentora ha aprovat el disseny.

**Següent:** [Sessió 6. Preparació per a la impressió (laminació)](s06-laminacio-cura.md)
