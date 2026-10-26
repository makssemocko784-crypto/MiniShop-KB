---

type: ontology  
created: 2026-10-26  
tags:

- minishop
    
- ontology
    

---

# Онтологія MiniShop

## Типи сутностей

- concept — поняття предметної області.
    
- component — програмний компонент.
    
- decision — архітектурне рішення.
    
- glossary — термін або визначення.
    

## Типи зв'язків

- depends_on — компонент залежить від іншого компонента.
    
- implements — компонент реалізує функціональність.
    
- uses — компонент використовує інший компонент.
    
- defined_by — компонент визначається архітектурним рішенням.
    

## Конвенція запису

Типізовані зв'язки записуються у YAML frontmatter з використанням англійських назв файлів без розширення .md.

Приклад:

depends_on:

- ShopLogic
    

defined_by:

- CLIArchitecture
    

## Приклади зв'язків

- [[CLI]] uses [[ShopLogic]].
    
- [[ShopLogic]] uses [[DataStorage]].
    
- [[DataStorage]] defined_by [[JSONStorage]].
    
- [[ShopLogic]] implements [[FunctionalRequirements]].