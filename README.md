# 🎁 Lista de Presentes Interativa — 15 Anos da Bárbara

Uma aplicação web elegante, responsiva e em tempo real concebida para gerir a lista de presentes da festa de 15 anos da Bárbara. O sistema permite que os convidados explorem sugestões divididas por categorias, visualizem galerias de imagens ou links diretos, e "reservem" o estilo de presente que desejam oferecer, com sincronização instantânea na nuvem.

## ✨ Funcionalidades Principais

- **Navegação por Categorias**: Menu principal intuitivo (`index.html`) que encaminha os convidados para secções específicas (Roupas, Calçados, Bolsas & Acessórios, e Beleza).
- **Galerias de Imagens Interativas**: Carrossel nativo desenvolvido em JavaScript Vanilla, permitindo aos utilizadores visualizar várias fotografias de uma mesma sugestão de presente antes de a escolherem.
- **Reservas em Tempo Real**: Integração com o **Firebase Realtime Database**. Quando um convidado insere o seu nome e confirma a escolha, o registo é guardado instantaneamente e o item passa a exibir uma etiqueta dinâmica (ex: `👥 Escolhido por 1 pessoa ✓`).
- **Sistema Híbrido de Sugestões**: Suporte tanto para itens com imagens locais (para demonstrar o estilo desejado) como para itens com links diretos para lojas externas (e-commerce).
- **Feedback Visual (UI/UX)**: Implementação de *Toast Notifications* elegantes que surgem no ecrã para confirmar o sucesso da reserva, além de um estado de *Loading* (spinner) enquanto os dados são obtidos da base de dados.
- **Design Temático e Responsivo**: Interface focada no utilizador móvel (*Mobile-First*), com uma paleta de cores personalizada em tons rosê e elementos de tipografia clássica e moderna.

## 🛠️ Tecnologias Utilizadas

- **Front-end**: HTML5, CSS3, JavaScript (ES6 Modules)
- **Base de Dados**: Firebase Realtime Database (SDK v10+)
- **Tipografia**: Google Fonts (`Urbanist`, `Playfair Display`, `Lato`)
- **Arquitetura**: Sistema modular de ficheiros estáticos (sem necessidade de frameworks complexas ou compiladores).

## 📂 Estrutura de Ficheiros

```text
/
├── index.html        # Menu principal (Vitrine de categorias)
├── roupas.html       # Lista de roupas (Calças, Leggings, Croppeds)
├── calcados.html     # Lista de calçados (Botas e Coturnos)
├── bolsas.html       # Lista de bolsas práticas e acessórios (Colares)
├── beleza.html       # Sugestões de Maquilhagem e Skincare
├── boticario.html    # Secção exclusiva para produtos d'O Boticário e QDB
└── img/              # Diretório contendo todas as imagens (.png/.jpg)
    ├── calcados/
    ├── roupas/
    ├── colar/
    └── logo_mateus.png