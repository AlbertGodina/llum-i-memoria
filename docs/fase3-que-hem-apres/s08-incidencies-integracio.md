# Sessió 8: Resolució d'incidències i integració física

!!! abstract "Dades de la sessió"
    **Durada:** 55 minuts · **Agrupament:** parelles

    **Objectiu:** muntar definitivament el circuit dins la capsa, integrar-hi la litofania i resoldre els problemes que hagin sortit del disseny o de la impressió.

## El prototip ja existeix

Ja teniu les peces impreses i el circuit provat. Avui les ajunteu. El producte encara no és acabat, però ha de **funcionar**. En aquesta fase consolideu el que heu après: no es tracta només de fer-ho funcionar, sinó d'entendre **per què funciona** i **com heu superat els obstacles**.

Aquesta sessió és clau per al portafoli: les incidències que resoleu avui seran una part important de la vostra història.

!!! info "Què es valora avui"
    Sobretot, **com detecteu i corregiu els problemes en parella**, de manera col·laborativa i repetint les proves fins que funciona. No es penalitza equivocar-se: es valora què en feu.

## Les quatre activitats

| Bloc | Què fem | Temps | Com |
|---|---|---|---|
| 1 | Inspecció de qualitat de les peces | 10 min | Parelles |
| 2 | Acabats després de la impressió | 15 min | Parelles |
| 3 | Integració electrònica i mecànica | 20 min | Parelles |
| 4 | Diari de bitàcola: registre d'errors | 10 min | Individual, dins la parella |

## 1. Inspecció de qualitat de les peces (10 min)

**Parelles.** Recolliu les peces impreses (litofania, cos i tapa) i reviseu-les críticament.

### Què hem de buscar

| Defecte | Com es veu |
|---|---|
| **Deformació** (*warping*) | Les cantonades s'han aixecat de la placa |
| **Restes** de vora o de suports | Hi ha plàstic enganxat, sobretot a la base de la litofania o a prop de la finestra |
| **Mides incorrectes** | La litofania no entra a l'encaix, hi va massa justa o hi balla; el tac de la tapa no entra a la cavitat |

Consulteu les [fitxes visuals](../recursos/fitxes-visuals.md) per comparar una deformació amb una impressió perfecta.

### Classifiqueu cada peça

| | Què vol dir | Què fem |
|---|---|---|
| ✅ | **Apta per muntar** | Continuem |
| ⚠️ | **Requereix retocs** | La podem arreglar nosaltres |
| ❌ | **Cal reimprimir** | Informeu el docent immediatament |

!!! warning "Una reimpressió és l'últim recurs"
    Només hi ha una impressora i la cua és llarga. Abans de demanar una reimpressió, pregunteu-vos si es pot arreglar amb un retoc. Una reimpressió es reserva per als defectes que impedeixen que la peça funcioni. El docent ho decidirà amb vosaltres.

**Producte:** la **checklist d'inspecció** completada per la parella.

## 2. Acabats després de la impressió (15 min)

**Parelles.** L'acabat manual és part del valor afegit d'un producte fet a mà.

1. **Retireu la vora** (*brim*) de la base de la litofania i les restes de suports, si n'hi ha, amb **pinces planes** o un **bisturí**. Treballeu sempre en direcció contrària al cos.
2. Si hi ha imperfeccions a la cara visible de la litofania, podeu suavitzar-les lleugerament amb **paper de vidre fi** (gra superior a 400, millor humit). **Aneu amb molta cura:** el relleu és el que forma la imatge, i si l'esborreu també canvieu la llum.
3. Si l'encaix de la litofania va massa just, **llimeu una mica la vora de l'encaix** de la capsa, no la litofania.
4. **Netegeu la pols** que heu generat.

!!! warning "Seguretat"
    Porteu **ulleres de protecció** i talleu sempre allunyant el bisturí del cos. Si no esteu segurs, demaneu ajuda al docent.

!!! info "Metodologia maker"
    Ara teniu tres maneres de resoldre un problema: **retocar a mà**, **tornar a Tinkercad** per corregir el disseny, o **tornar a Bambu Studio** per ajustar els paràmetres. Pensem sempre quina és la més ràpida i la que gasta menys material.

**Producte:** les peces netes, sense restes i preparades per al muntatge.

## 3. Integració electrònica i mecànica (20 min)

**Parelles.** Aquests passos són per ordre.

1. **Passeu el cable per la tapa.** Desconnecteu la tira del cable (és fàcil si heu fet servir connectors de clip). Passeu l'extrem del cable pel **forat de 5 mm** de la tapa, **de fora cap a dins**. El connector USB queda a fora.
2. **Feu un nus al cable**, a la banda de dins de la tapa. Així, si algú estira el cable, la connexió de la tira no es desfarà.
3. **Torneu a connectar** el cable a la tira, amb l'interruptor si en porteu. Reviseu que els fils no es toquin.
4. **Fixeu la tira** a la cara interior del tac de la tapa, amb la disposició que vau provar a la sessió 7. Si la tira és autoadhesiva, només cal premre-la. Si no, podeu fer servir cinta de doble cara o silicona calenta, si el docent ho permet.
5. **Inseriu la litofania** a l'encaix de la capsa, **pel darrere** i amb la tapa oberta. Ha de quedar ben assentada i centrada darrere la finestra.
6. **Tanqueu la tapa**: empenyeu el tac dins la cavitat sense forçar.
7. **Prova funcional final.** Endolleu el cable a una font d'alimentació (ordinador o carregador). Apagueu els llums de l'aula o feu servir una caixa fosca improvisada i comproveu que la imatge es projecta amb claredat.

!!! tip "La imatge surt girada com en un mirall"
    Si un text o una imatge es veu invertit, la litofania està girada. Gireu-la pel davant i pel darrere. Si això no ho soluciona, torneu-la a generar a [tool.itslitho.com](https://tool.itslitho.com/) amb l'opció **Mirror**.

### Si la imatge es veu borrosa o fosca

Penseu-hi com a enginyers i enginyeres. Revisareu aquestes possibles causes, d'una en una:

- [ ] La **tira és massa a prop** de la litofania i es veuen **franges o punts de llum**? Proveu a posar-hi un full de **paper vegetal** entre la tira i la litofania per difondre la llum.
- [ ] La **tira és massa lluny** o la llum no arriba a tota la imatge? Proveu una altra disposició de les files.
- [ ] Hi ha **llum que s'escapa pels costats** de la capsa? Podeu segellar-ho amb cinta negra.
- [ ] El **contrast de la foto original** era insuficient? Això només es resol amb una nova litofania.

!!! warning "Comproveu l'escalfament"
    Després d'uns minuts amb la llum encesa, **toqueu la capsa i la tapa**: no s'han d'escalfar. Si noteu calor, desendolleu i aviseu el docent.

**Producte:** el **prototip funcional**, muntat i verificat.

## 4. Diari de bitàcola: registre d'errors (10 min)

**Individual, dins la parella.** Cadascú escriu (o grava una nota de veu) sobre **un error concret** que heu trobat avui i **com s'ha solucionat**.

!!! example "Exemple"
    «El tac de la tapa no entrava a la cavitat perquè havia oblidat el joc de 0,4 mm. He llimat les vores del tac amb la lima i ara hi entra.»

!!! tip "Altres formats"
    Si escriure us costa, podeu fer un **mapa mental visual** o una **nota de veu** curta.

**Producte:** una entrada al diari de projecte compartit.

## Abans de marxar

- [ ] Hem classificat les peces (✅ ⚠️ ❌).
- [ ] Hem fet els acabats necessaris.
- [ ] Tenim el prototip muntat i funcionant.
- [ ] Hem escrit el registre d'un error al diari.

**Següent:** [Sessió 9. Documentació digital i assajos de comunicació](s09-portafoli-digital.md)
