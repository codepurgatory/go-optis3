<img alt="git-readme-header" src="assets/git-readme-header.png" height="320" />

![Static Badge](https://img.shields.io/badge/PROJECT_STATUS-In_development-9B59B6?logo=statuspal&style=for-the-badge)
![Static Badge](https://img.shields.io/badge/GO-Project/MicroServices-00E2FF?logo=go&style=for-the-badge)
![Static Badge](https://img.shields.io/badge/Pattern-SOLID-00E2FF?logo=solid&style=for-the-badge)

![Static Badge](https://img.shields.io/badge/DOCKER-SUPPORT-blue?logo=DOCKER&style=for-the-badge)
![Static Badge](https://img.shields.io/badge/GOLAND_IDE-USE_FOR_DEVELOPMENT-white?logo=goland&style=for-the-badge)

<details>
<summary><strong>Project Design Principles</strong></summary>
  <div>
  
  ## Project Design Principles
  #### SOLID is an acronym for the five principles of object-oriented programming. These principles help create code that is clear, flexible, and easy to maintain.
  * ![Static Badge](https://img.shields.io/badge/S-—_Single_Responsibility_Principle-white?logo=solid&style=for-the-badge)
  * ![Static Badge](https://img.shields.io/badge/O-—_Open/Closed_Principle-white?logo=solid&style=for-the-badge)
  * ![Static Badge](https://img.shields.io/badge/L-—_Liskov_Substitution_Principle-white?logo=solid&style=for-the-badge)
  * ![Static Badge](https://img.shields.io/badge/I-—_Interface_Segregation_Principle-white?logo=solid&style=for-the-badge)
  * ![Static Badge](https://img.shields.io/badge/D-—_Dependency_Inversion_Principle-white?logo=solid&style=for-the-badge)
  
  ### Folders:
  * `config` → **Configuration**  
    Application configuration (env variables, YAML, settings)
  
  * `handlers` → **HTTP Handlers / Controllers**  
    Entry points for incoming requests (API layer)
  
  * `interfaces` → **Interfaces / Contracts**  
    Contracts for core components (e.g., Storage, ImageProcessor)
  
  * `middleware` → **Middleware**  
    Request/response interceptors (auth, logging, rate limiting)
  
  * `models` → **Domain Models**  
    Internal data structures (e.g., Image, User)
  
  * `providers` → **Providers / Integrations**  
    External implementations (e.g., S3, local storage, image processing)
  
  * `services` → **Business Logic / Services**  
    Core application logic (facade + use cases)
  
  * `utils` → **Utilities / Helpers**  
    Helper functions (files, errors, small utilities)
  
    ### Relationships
    `handlers` → `services` → `interfaces` ← `providers`
    </div>
</details>
