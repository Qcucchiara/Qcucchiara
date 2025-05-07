## Bonjour, Je suis Phost, développeur web et concepteur développeur d'application en devenir
je suis actuellement à la recherche d'un stage de 5 mois entre le 8 septembre 2025 et le 16 janvier 2026 dans le cadre de ma formation.

## Stack Technique
```text
│────────────────│   │─────────────────│   │──────────────│   │───────────────│
│  Frameworks    │   │  Libraries      │   │  DevOps      │   │  Databases    │
│────────────────│   │─────────────────│   │──────────────│   │───────────────│
│ ► Next.js      │   │ ► Node.js       │   │ ► Docker     │   │ ► MongoDB     │
│ ► React Native │   │ ► Express       │   │ ► GitLab CI  │   │ ► PostgreSQL  │
│ ► NestJS       │   │ ► React         │   │ ► Apache2    │   │ ► MySQL       │
│ ► Symfony      │   │ ► Tailwind CSS  │   │──────────────│   │───────────────│
│────────────────│   │─────────────────│

│────────────────│   │───────────────────────│    │────────────│
│  Languages     │   │  Tools                │    │  Design    │    
│────────────────│   │───────────────────────│    │────────────│    
│ ► French       │   │ ► Git                 │    │ ► Figma    │    
│ ► English      │   │ ► GitHub              │    │ ► Canva    │    
│ ► Javascript   │   │ ► GitLab              │    │ ► Blender  │    
│ ► TypeScript   │   │ ► Visual Studio Code  │    │────────────│    
│ ► CSS          │   │ ► IntelliJ JetBrains  │    
│ ► HTML         │   │ ► Postman             │
│ ► SQL          │   │ ► Trello              │
│ ► Java         │   │ ► Discord             │
│ ► Kotlin       │   │───────────────────────│
│ ► C#           │
│ ► PHP          │
│────────────────│
```
## 🔭 Je développe sur mon temps libre un moteur de jeu 2d avec architecture ECS
```mermaid
classDiagram
    class IdManager {
        -currentIdCount: number
        -freeIds: number[]
        -getNextId(): number
        +allocateId(): number
        +freeId(id: number): void
    }
    
    class ComponentManager {
        -instance: ComponentManager
        -registeredComponents: Map<string, Class>
        +getInstance(): ComponentManager
        +register(name: string, class: Class): boolean
        +create(name: string): AbstractComponent
    }
    
    class EntityManager {
        -idManager: IdManager
        -componentManager: ComponentManager
        -entities: Iterable<Array<Component>>
        +setEntity(): Iterable<Array<Component>>
        +removeEntity(id): boolean
        +getEntities(): Iterable<Array<Component>>
        +addComponent(entityId: number, component: Component): boolean
        +getComponents(entityId: number): Array<Component>
        +removeComponent(entityId: number): boolean
    }
    
    class ECS {
        -instance: ECS
        +entityManager: EntityManager
        +componentManager: ComponentManager
        -systems: Set<ISystem>
        +getInstance(): ECS
        +addSystem(system: AbstractSystem): boolean
        +update(): void
    }
    
    class ISystem {
        <<Interface>>
        +update(deltaTime: number): void
    }
    
    IdManager <-- EntityManager
    ComponentManager <-- EntityManager
    ComponentManager <-- ECS
    EntityManager <-- ECS
    ISystem <-- ECS
    
    EntityManager "1" -- ECS
```

<!-- 
<div align="center">
     <img src="Screenshot From 2025-05-07 19-15-21.png" border="0">
</div>
-->

- 🌱 J'apprend actuellement l'architecture ECS, la méthodologie scrum et devops 
- 👯 Mon objectif final est d'intégrer une équipe en tant qu'architecte logiciel
- 🤔 Je recherche un accompagnement pour m'aider à monter en compétence et je pourrais apporter mon esprit de sorcier aiguisée 
- 📫 Vous pouvez me contacter par mail à l'adresse: cucchiaraquentin@gmail.com
- ⚡ Euhhh ... je sais plus ce que je voulais dire ...
