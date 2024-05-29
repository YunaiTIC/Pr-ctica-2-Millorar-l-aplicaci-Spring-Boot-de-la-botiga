# Botiga DAM2

Aquest projecte és una aplicació web desenvolupada amb Spring Boot que gestiona una botiga en línia. Les funcionalitats inclouen la gestió de categories, subcategories i productes, així com la cerca de productes per nom.

## Estructura del projecte

El projecte està dividit en diversos paquets per a una millor organització del codi:

- `Controller`: Conté els controladors que gestionen les peticions HTTP.
- `Model`: Conté les entitats que representen les dades de la base de dades.
- `Repositori`: Conté les interfícies de repositori per a l'accés a les dades.
- `Service`: Conté les interfícies dels serveis.
- `Service.impl`: Conté les implementacions dels serveis.

## Fitxers importants

- `WebController.java`: Controlador principal que gestiona les peticions de la pàgina web.
- `Category.java`, `Subcategory.java`, `Product.java`: Entitats que representen les categories, subcategories i productes respectivament.
- `CategoryRepository.java`, `SubcategoryRepository.java`, `ProductRepository.java`: Repositoris per a l'accés a les dades.
- `CategoryServiceImpl.java`, `SubcategoryServiceImpl.java`, `ProductServiceImpl.java`: Implementacions dels serveis.
- `index.html`, `catalog.html`, `product_form.html`, `search.html`: Pàgines HTML per a la interfície d'usuari.

## Instal·lació

1. Cloneu el repositori: `git clone https://github.com/usuari/botiga-dam2.git`
2. Navegueu fins al directori del projecte: `cd botiga-dam2`
3. Executeu l'aplicació: `./mvnw spring-boot:run`

## Proves

Les proves es poden realitzar accedint a les diferents pàgines de l'aplicació web:

1. **Pàgina d'inici**: Accediu a `http://localhost:8080` per veure la pàgina principal.
2. **Catàleg de productes**: Accediu a `http://localhost:8080/catalog` per veure el catàleg de productes.
3. **Formulari de nou producte**: Accediu a `http://localhost:8080/createProduct` per veure el formulari d'inserció de productes.
4. **Cerca de productes**: Accediu a `http://localhost:8080/search` per cercar productes pel seu nom.

