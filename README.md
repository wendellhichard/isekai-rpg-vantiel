# Isekai RPG: Vantiel — Uma Aventura Potencializada por IA

Bem-vindo ao repositório do **Isekai RPG: Vantiel**, um projeto de RPG de texto interativo projetado para ser mestrado por uma IA personalizada, construída com o Google Gemini.

Este repositório não contém o código de um jogo tradicional, mas sim a **base de conhecimento (knowledge base)** que serve como o "cérebro" e a "memória" do Mestre de Jogo (Game Master) de IA.

## 🚀 O Conceito

O objetivo deste projeto é criar uma experiência de RPG rica e consistente, onde um modelo de linguagem (Gemini) atua como narrador e árbitro das regras. Para evitar que a IA "alucine" ou invente regras, nós fornecemos a ela uma biblioteca de conhecimento bem estruturada.

O Gem utiliza uma técnica chamada **RAG (Retrieval-Augmented Generation)**. Em vez de usar apenas seu conhecimento geral, ele primeiro busca as informações relevantes nos arquivos deste repositório e, em seguida, gera a resposta com base nesse contexto. Isso garante que o mundo de Vantiel permaneça coeso e que as regras sejam aplicadas de forma justa.

## 📂 Estrutura do Repositório

O conhecimento do Gem está inteiramente contido na pasta `knowledge_base/`. A organização é projetada para ser modular e fácil de entender, tanto para humanos quanto para a IA.

-   **/knowledge_base/**: A biblioteca central de todo o conhecimento do jogo.
    -   `01_core_rules/`: Contém as regras fundamentais e imutáveis do jogo, como criação de personagem, o sistema de dados e os princípios básicos.
    -   `02_mechanics/`: Descreve todos os sistemas de jogo: combate, habilidades, magias, crafting, economia, etc. Cada mecânica possui seu próprio arquivo para garantir precisão.
    -   `03_world_lore/`: Detalha o mundo de Vantiel. Aqui você encontrará informações sobre a história, locais, facções, NPCs importantes e o bestiário.
    -   `04_examples_and_templates/`: Fornece exemplos concretos e modelos que a IA usa como referência para narrar sessões e estruturar informações, como fichas de personagem e receitas de crafting.

-   **/deployment/**: Contém os arquivos necessários para configurar o Gem.
    -   `prompt_instructions.md`: Este é o arquivo mais importante. Ele funciona como o "manual de instruções" da IA, definindo sua personalidade, seus objetivos e, o mais importante, a diretiva para usar a `knowledge_base/` como sua única fonte de verdade.

## 🛠️ Como Contribuir ou Modificar

A beleza deste sistema é a facilidade de modificação e expansão. Para alterar ou adicionar conteúdo ao jogo, basta editar os arquivos de texto:

-   **Para modificar uma regra:** Encontre o arquivo `.md` correspondente na pasta de mecânicas ou regras e faça sua alteração.
-   **Para adicionar um novo monstro:** Adicione uma nova entrada no arquivo `bestiary.md` na pasta de lore.
-   **Para criar uma nova cidade:** Adicione uma descrição no arquivo de locais apropriado.

O segredo é manter a consistência e garantir que as novas informações não contradigam o que já foi estabelecido.

## 📄 Licença

Este projeto é distribuído sob a licença contida no arquivo [LICENSE](LICENSE).
