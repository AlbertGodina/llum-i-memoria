# Sessió 7: Inici de la fabricació i muntatge electrònic

!!! abstract "Dades de la sessió"
    **Durada:** 55 minuts · **Agrupament:** parelles

    **Objectiu:** muntar el circuit de llum amb una tira LED i un cable USB reciclat, mentre la impressora fabrica les peces.

## Aprofitem l'espera

Les peces ja són a la cua d'impressió, i la impressora triga. Mentrestant, muntareu la part elèctrica del producte: un circuit que dona vida a la litofania. Farem servir **materials reciclats** i una **tira LED de 5 V** alimentada per un **cable USB** que ja no feia servei.

Recordeu que en el món maker, si alguna cosa no funciona, no es busquen culpables: es busca l'error.

## Les quatre activitats

| Bloc | Què fem | Temps | Com |
|---|---|---|---|
| 1 | Recollim els materials | 10 min | Parelles |
| 2 | Esquema final i càlcul del consum | 10 min | Parelles |
| 3 | Muntatge i prova del circuit | 30 min | Parelles |
| 4 | Integració preliminar | 5 min | Parelles |

## 1. Recollim els materials (10 min)

**Parelles.** Agafeu el **kit de materials reciclats** i prepareu l'estació de treball.

| Material | Per a què serveix |
|---|---|
| **Cable USB reciclat** | Porta l'energia de 5 V. El fil vermell és el **+5 V** i el negre és la **massa (GND)** |
| **Tira LED de 5 V** | És la font de llum |
| **Interruptor** (opcional) | Per encendre i apagar la llum |
| **Connectors de clip** per a tira LED, o **soldador** | Per unir els fils a la tira |
| **Pelacables o tisores, cinta aïllant o termoretràctil** | Per preparar i aïllar les connexions |
| **Multímetre** (opcional) | Per comprovar cables i mesurar el consum |

!!! warning "Seguretat"
    - Porteu **ulleres de protecció** quan talleu plàstic dur o treballeu amb el soldador.
    - El soldador crema: només el podeu fer servir si el docent ho permet.
    - **Mentre munteu, el cable USB ha d'estar desendollat.**

**Producte:** els components ben ordenats a la taula.

## 2. Esquema final i càlcul del consum (10 min)

**Parelles.** Aquest és el circuit que construireu:

```
   + 5 V (fil vermell) ──── [ interruptor ] ──── (+) TIRA LED
   GND   (fil negre)   ───────────────────────── (−) TIRA LED
```

A la sessió 2 vau calcular la resistència d'**un** LED. Una tira LED és com molts LED, cadascun amb la seva resistència ja soldada, connectats en paral·lel. Per això aquí **no cal afegir cap resistència**.

### Quant consumeix?

La font USB no pot donar tot el corrent que vulgueu. Cal saber què consumeix la vostra tira i comprovar que la font ho aguanta.

1. Mireu les dades de la tira (a l'etiqueta o a la bobina): el **corrent o la potència per metre**.
2. Decidiu quants **centímetres** en farà servir la vostra litofania. Només es pot tallar per les **marques de tall** que porta la tira.
3. Calculeu el corrent i la potència del tros que fareu servir:

    **I = corrent per metre × longitud en metres**

    **P = V · I**, amb V = 5 V

    *Exemple: una tira de 0,5 A per metre, amb 20 cm (0,2 m) → I = 0,5 × 0,2 = 0,1 A (100 mA) i P = 5 × 0,1 = 0,5 W. Heu de fer el càlcul amb les dades de la vostra tira.*

4. Comproveu que la font de 5 V ho pot donar. Un port USB d'ordinador sol donar uns 500 mA, i un carregador, més.

**Producte:** l'**esquema elèctric final** (net, amb símbols estàndard) i el **càlcul del consum** de la vostra tira.

## 3. Muntatge i prova del circuit (30 min)

**Parelles.** Aquests passos són per ordre.

!!! tip "El cable USB: fils molt fins"
    Els fils dels cables USB són molt prims i es trenquen amb facilitat. Peleu-los amb cura.

1. **Talleu la tira.** Només per les marques de tall. Podeu provar diferents disposicions: un sol tros recte o dos trossos paral·lels.
2. **Prepareu el cable USB.** Talleu l'extrem que no és l'endoll USB i retireu uns **5 mm** d'aïllament de cada fil. Torçeu els fils de coure.
3. **Identifiqueu els fils.** El **vermell** és el +5 V i el **negre** és la massa. Els altres dos (blanc i verd) són de dades i no els fem servir: **aïlleu-los** amb cinta.

    ??? tip "Si els colors no coincideixen"
        No tots els cables reciclats segueixen els colors estàndard. Demaneu al docent que us ajudi a identificar el +5 V amb el multímetre.

4. **Connecteu el fil vermell a la tira.** Si feu servir interruptor, poseu-lo entre el fil vermell i la tira. Feu servir un connector de clip o soldeu amb cura.
5. **Connecteu el fil negre a la tira**, al costat marcat amb el signe **−**.
6. **Aïlleu** totes les unions amb cinta o termoretràctil. Eviteu qualsevol contacte entre fils pelats: això és un curtcircuit.
7. **Proveu el circuit.** Endolleu el USB a un port de càrrega (ordinador o carregador). La tira s'ha d'encendre. Si no ho fa, desendolleu i reviseu les connexions.

!!! info "Metodologia maker: si falla, busqueu l'error"
    No culpeu el component. Pot ser una **polaritat invertida** (+ i − girats), una **mala connexió** o un **fil trencat**. Documenteu què era i com ho heu solucionat: servirà per al portafoli.

!!! warning "Comproveu l'escalfament"
    Després d'uns minuts de funcionament, toqueu amb cura els fils: **no s'han d'escalfar**. Si s'escalfen, desendolleu immediatament i aviseu el docent.

!!! success "Repte per pensar"
    A la sessió 8 col·locareu la tira dins de la capsa, darrere de la litofania. **Com repartiríeu la llum perquè la imatge es vegi uniforme?** Podeu provar diferents disposicions de la tira sobre un cartró de 80 × 60 mm, sense enganxar-la encara.

**Producte:** el **circuit funcionant** fora de la capsa i una **foto del muntatge net**.

## 4. Integració preliminar (5 min)

**Parelles.**

1. Comproveu si les peces impreses ja han sortit de la impressora.
2. Si sí, proveu d'introduir la tira i els cables dins la capsa, per veure si hi caben còmodament.
3. Si no, guardeu el circuit amb cura per a la sessió 8.

**Producte:** una actualització de l'estat del projecte al diari digital.

## Abans de marxar

- [ ] Tenim l'esquema final i el càlcul del consum.
- [ ] El circuit s'encén i funciona.
- [ ] Hem aïllat totes les connexions.
- [ ] Hem fet la foto del muntatge net.
- [ ] Hem apuntat al diari els errors i les solucions.

**Següent:** [Sessió 8. Resolució d'incidències i integració física](../fase3-que-hem-apres/s08-incidencies-integracio.md)
