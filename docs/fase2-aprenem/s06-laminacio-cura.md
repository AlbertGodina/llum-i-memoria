# Sessió 6: La impressora 3D i la laminació

!!! abstract "Dades de la sessió"
    **Durada:** 55 minuts · **Agrupament:** grup classe i parelles

    **Objectiu:** conèixer com funciona la impressora 3D de l'aula i configurar al laminador els paràmetres bàsics per imprimir la litofania i la capsa amb qualitat.

## De l'arxiu digital a la peça física

Tot el que heu dissenyat és encara digital. Avui coneixereu la màquina que ho farà realitat, una **Bambu Lab P2S**, i prepareu els arxius perquè pugui imprimir-los.

La impressió la farà el docent, però **vosaltres decidiu els paràmetres** que determinen la qualitat de les peces. Un bon ajust ara us estalviarà temps i material més endavant.

## Les quatre activitats

| Bloc | Què fem | Temps | Com |
|---|---|---|---|
| 1 | Com funciona la impressora | 10 min | Grup classe |
| 2 | Exportem i importem a Bambu Studio | 10 min | Parelles |
| 3 | Configurem els paràmetres bàsics | 25 min | Parelles |
| 4 | Enviament i cua d'impressió | 10 min | Grup classe |

## 1. Com funciona la impressora (10 min)

**Grup classe.** El docent us mostra la impressora. Busqueu cada part a la màquina:

| Part | Què fa |
|---|---|
| **Tovera** (*nozzle*) de 0,4 mm | Escalfa i fon el plàstic i el diposita. El seu diàmetre limita el detall que es pot imprimir |
| **Filament** (la bobina de PLA) | És el material. Entra pel capçal i es fon a la tovera |
| **Placa d'impressió** | Hi comença la peça. S'escalfa una mica perquè la primera capa s'hi enganxi |
| **Cambra tancada** | Manté l'aire estable i protegeix la peça dels corrents |
| **Pantalla tàctil i càmera** | Serveixen per controlar la impressora i seguir la impressió |

### Què passa quan premem «imprimir»?

1. El **laminador** talla el model en capes molt fines i en genera les instruccions.
2. La impressora **escalfa** la tovera i la placa.
3. Fa uns **calibratges automàtics** abans de començar.
4. **Diposita el plàstic capa a capa**, de baix cap a dalt.
5. Quan acaba, la peça es refreda i se separa de la placa.

!!! warning "Seguretat"
    La tovera arriba a uns 220 °C i la placa també s'escalfa. **No toqueu res de dins** de la impressora, ni en funcionament ni just després. No obriu la porta durant la impressió.

!!! question "Per pensar"
    Per què creieu que imprimir amb capes més fines fa que la peça trigui més?

## 2. Exportem i importem a Bambu Studio (10 min)

**Parelles.** El **laminador** que fem servir és **Bambu Studio**, el programa de la impressora.

### Els arxius que necessiteu

- **Litofania:** ja la teniu en STL, la de la [sessió 1](../fase1-que-en-sabem/s01-repte-ideacio.md). Si en algun moment l'heu modificada a Tinkercad, torneu-la a exportar.
- **Cos i tapa de la capsa:** exporteu-los des de Tinkercad. Seleccioneu només la peça que voleu, premeu **Export** i trieu **.STL**. Poseu-los noms clars: `cos` i `tapa`.

### Prepareu dos projectes

Cada parella farà **dos projectes** a Bambu Studio, perquè la litofania i la capsa necessiten ajustos diferents:

| Projecte | Què hi poseu |
|---|---|
| `Parella_X_litofania` | La litofania |
| `Parella_X_capsa` | El cos i la tapa |

1. Obriu Bambu Studio i trieu la impressora **Bambu Lab P2S** amb tovera de 0,4 mm.
2. Importeu els fitxers STL (**Ctrl + I**).
3. Orienteu les peces tal com s'indica a continuació.

### L'orientació de cada peça

| Peça | Com la posem | Per què |
|---|---|---|
| **Litofania** | **Dreta, vertical**: apoiada sobre el cantell | La resolució horitzontal és molt més fina, i això defineix la imatge |
| **Cos** | Amb la **cara del davant** (la de la finestra) sobre la placa, i el darrere cap amunt | No necessita suports, perquè cada capa és més estreta que l'anterior |
| **Tapa** | **Plana**, amb el tac cap amunt | També sense suports |

!!! tip "Eines per orientar"
    Premeu **F** (*Place on face*) i feu clic a la cara que voleu posar sobre la placa. Per girar la peça, feu servir l'eina de rotació (**R**).

## 3. Configurem els paràmetres bàsics (25 min)

**Parelles.** Premeu l'interruptor **Advanced** (mode avançat) del panell de processos per veure tots els paràmetres. Primer configureu la litofania i després la capsa.

| Paràmetre | Què controla | Litofania | Capsa (cos i tapa) |
|---|---|---|---|
| **Alçada de capa** (*Layer height*) | El gruix de cada capa. Com més petita, més detall i més temps | **0,1 mm** | **0,2 mm** |
| **Ompliment** (*Sparse infill density*) | El percentatge de l'interior que s'omple de plàstic | **100 %** | **15 %** |
| **Patró d'ompliment** (*Sparse infill pattern*) | La forma de l'ompliment | **Rectilinear** | El que ve per defecte |
| **Velocitat de la paret exterior** (*Outer wall speed*) | La rapidesa amb què es fa el contorn | **Baixa, uns 50 mm/s** | El que ve per defecte |
| **Vora** (*Brim*), pestanya *Others* | Una base més ampla que ajuda la peça a no moure's | **Sí** | No |
| **Suports** (*Support*) | Estructures temporals per sostenir parts que queden en l'aire | **No**, tret que sigui imprescindible | **No** |
| **Filament** | El material | **PLA blanc** (no mat, ni negre, ni transparent) | PLA de qualsevol color |

??? tip "Si no trobeu 0,1 mm a la llista"
    Els perfils de Bambu Studio porten alçades de capa estàndard. Podeu escriure els **0,1 mm** a mà al paràmetre *Layer height*.

### Per què aquests valors per a la litofania?

- **Vertical i capa fina.** Imprimir la litofania dreta i amb capes de 0,1 mm dona molta més nitidesa. La contrapartida és que **triga més** i la peça és prima i alta, així que cal una **vora** perquè no es mogui.
- **Ompliment al 100 %.** Si l'interior fos buit o amb una graella, es veurien ombres a la imatge. Volem que sigui plàstic sòlid i uniforme.
- **PLA blanc.** El plàstic ha de deixar passar la llum de manera uniforme. El mat difusa la llum d'una altra manera i en perjudica el contrast.

!!! info "Per què la capsa es fa més ràpid?"
    La capsa no necessita detall: només ha de ser resistent. Amb capes de 0,2 mm i un 15 % d'ompliment gasteu menys plàstic i menys temps.

### Reviseu la previsualització

1. Premeu **Slice plate** (laminar la placa).
2. Moveu el control lliscant de capes de la dreta per veure com es construeix la peça capa a capa.
3. Comproveu que **no hi ha parts flotants** i que la litofania té vora.
4. Anoteu a la taula el **temps estimat** i els **grams de PLA** que mostra el programa.

| Peça | Temps estimat | Plàstic (g) |
|---|---|---|
| Litofania | | |
| Cos | | |
| Tapa | | |
| **Total** | | |

!!! question "Per pensar"
    Quina peça triga més? Per què? Què passaria amb el temps total si la litofania es fes amb capes de 0,2 mm?

**Producte:** els dos projectes de Bambu Studio, la **taula de temps i consum**, i una **justificació breu** (escrita o oral) de la configuració de la litofania: per què vertical? Per què ompliment al 100 %?

## 4. Enviament i cua d'impressió (10 min)

**Grup classe.** Només hi ha **una impressora** i moltes parelles, per això cal ordre.

1. Deseu els projectes (`.3mf`) a la carpeta compartida de la classe, amb els noms `Parella_X_litofania` i `Parella_X_capsa`.
2. El docent organitza la **cua d'impressió** i us indica quan tindreu les peces.
3. Mentre s'imprimeix, passeu a la [sessió 7](s07-electronica-led.md) i munteu el circuit.

!!! info "Per què triguem tant?"
    Si sumeu els temps de totes les parelles, veureu que són moltes hores d'impressió. Per això la planificació del [cronograma de la sessió 2](../fase1-que-en-sabem/s02-planificacio-cicle-vida.md) era important.

**Producte:** la confirmació que els dos projectes són a la carpeta compartida.

## Abans de marxar

- [ ] Tenim els dos projectes preparats (litofania i capsa).
- [ ] Hem orientat les peces tal com toca.
- [ ] Hem anotat el temps estimat i els grams de PLA.
- [ ] Hem justificat la configuració de la litofania.
- [ ] Els projectes són a la carpeta compartida.

!!! tip "Si us encalleu"
    Demaneu ajuda al docent o a una parella mentor. Si l'avís de Bambu Studio parla de parts flotants a la litofania, no passa res si hi ha vora; comproveu-ho amb el docent.

**Següent:** [Sessió 7. Inici de la fabricació i muntatge electrònic](s07-electronica-led.md)
