# Funcionament de la prova:
**- Inici de la tasca: 15 d’abril.**
**- Data límit d’entrega: 30 d’abril.**
**- No es pot fer ús de cap intel·ligència artificial.**

# S'ha d'entregar: 
**- Projecte complet amb arxius HTML, JS i CSS.**
**- S'ha de poder veure a través de Github pages.**

# Enunciat:
**Desenvolupar una aplicació web modular que permeti planificar, gestionar i fer seguiment de tasques personals mitjançant formularis, visualització gràfica i persistència de dades. Aquesta aplicació simula un gestor personal d'activitats, posant en pràctica tots els coneixements apresos durant el curs.**

## Requisits i funcionaliats mínims:
L’aplicació ha d’estar composta per **3 pàgines HTML** amb les funcionalitats següents:

### index.html - Vista Principal
- Ha de tenir un menú de navegació.
- Mostra un **llistat de totes les activitats**.
- Permet:
    - **crear, eliminar, marcar com a realitzades**.
- Mostra un **gràfic amb Chart.js** amb les tasques realitzades per mes.
- Carrega les activitats des de:
    - localStorage.
    - un fitxer activitats.json (importació amb fetch(), evitant duplicats).

### crear-tasca.html - Formulari per afegir activitats
- Ha de tenir un menú de navegació.
- Inclou un formulari amb validació:
    - títol, descripció, data, categoria (selector de categories), prioritat (selector de Baixa, Mitjana, Alta).
- Guarda les activitats a localStorage amb un id únic amb el format "task-001" i el camp realitzada: false.

### categories.html - Gestor de categories
- Ha de tenir un menú de navegació.
- Permet afegir i eliminar categories que es poden usar al formulari.
- Les categories es guarden a localStorage.

## Organització del projecte:
PRACTICA_FINAL
    > css
        > style.css
    > dades
        > activitats_001.json
        > activitats_002.json
    > js
        > categories.js
        > form-tasca.js
        > grafics.js
        > index.js
        > models.js
        > storage.js
    > categories.html
    > crear-tasca.html
    > index.html

## Rúbrica: 
| Criteri                                     | Punts| HTML (20%) | CSS (20%) | JS (60%) |
|---------------------------------------------|------|------------|-----------|----------|
| Llistat i gestió de tasques (CRUD)          | 2    | 0.4        | 0.4       | 1.2      |
| Formulari funcional i validació             | 2    | 0.4        | 0.4       | 1.2      |
| Marcatge i gestió de tasques realitzades    | 1    | 0.2        | 0         | 0.8      |
| Gràfic funcional amb Chart.js               | 1    | 0.1        | 0.1       | 0.8      |
| Importació amb fetch() i JSON               | 1    | 0          | 0         | 1        |
| Gestió de categories                        | 1    | 0.2        | 0.2       | 0.6      |
| Estructura en mòduls i netedat de codi      | 1    | 0.1        | 0         | 0.9      |
| Disseny visual i usabilitat                 | 1    | 0.2        | 0.8       | 0        |
| **Total**                                   | **10** | **1.6**    | **2.0**   | **6.4**  |