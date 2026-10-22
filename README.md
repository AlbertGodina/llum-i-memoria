# Llum i Memòria: disseny 3D per a records il·luminats

Web de la situació d'aprenentatge (SDA) de **Tecnologia de 4t d'ESO** en què l'alumnat, organitzat en parelles que fan de startup, dissenya i fabrica una **litofania il·luminada amb LED i cable USB reciclat**.

El web guia l'alumnat sessió a sessió (12 sessions de 55 minuts): ideació, disseny 3D amb Tinkercad, laminació, electrònica bàsica, portafoli digital i pitch final.

## Estructura

```
docs/
├── index.md                 Presentació, repte i calendari
├── com-treballem.md         Parelles, rols, portafoli i avaluació
├── fase1-que-en-sabem/      Sessions 1 i 2
├── fase2-aprenem/           Sessions 3 a 7
├── fase3-que-hem-apres/     Sessions 8 i 9
├── fase4-apliquem/          Sessions 10 a 12
├── practica-tinkercad/      Banc d'exercicis de Tinkercad (5 blocs)
├── recursos/                Plantilles, fitxes visuals, enllaços de rescat, calculadora
├── extres/                  Capsa amb talladora làser (en preparació, fora del menú)
├── lliuraments.md
└── glossari.md
```

El material per al professorat (guió de sessions, rúbriques i ponderació, notes DUA, gestió de cues d'impressió) **no** és en aquest repositori públic.

## Veure el web en local

```bash
pip install -r requirements.txt
mkdocs serve
```

Obre <http://127.0.0.1:8000>.

## Publicació

Cada `push` a la branca `main` executa la GitHub Action *Deploy MkDocs to GitHub Pages*, que genera el web en mode estricte (`mkdocs build --strict`) i el publica. El build falla si hi ha enllaços o fitxers del menú que no existeixen.

Perquè funcioni, a **Settings → Pages** del repositori, la font ha de ser **GitHub Actions**.

## Crèdits

Basat en el *Taller de litofanies* de Xavi Perramon (Escola Pia Nostra Senyora, Barcelona), presentat a la XIa Jornada d'Innovació a l'Ensenyament de la Tecnologia (JIET).
