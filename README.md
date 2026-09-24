# 💧 Gás & Água - Delivery App (Android)

[![Kotlin](https://img.shields.io/badge/Kotlin-1.9%2B-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/)
[![Firebase](https://img.shields.io/badge/Backend-Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Architecture](https://img.shields.io/badge/Architecture-MVVM%20%2B%20Clean-blue?style=for-the-badge)]()

Aplicativo Android nativo para pedidos e entrega rápida de botijões de gás e galões de água mineral, desenvolvido como projeto final da disciplina de **Programação Orientada a Objetos (POO)**.

---

## 📱 Telas e Funcionalidades

* 🔐 **Autenticação Segura**: Login e cadastro de usuários via Firebase Authentication com validação de campos.
* 🛍️ **Catálogo de Produtos**: Navegação categorizada entre Água Mineral (diversas litragens/marcas) e Gás de Cozinha.
* 🛒 **Carrinho de Compras Interativo**: Adição/remoção de itens, controle dinâmico de quantidade e cálculo automático do total.
* 📍 **Gestão de Endereços**: Cadastro de múltiplos endereços de entrega com seleção no checkout.
* 📋 **Gestão de Pedidos**: Histórico de compras com status atualizado e detalhes dos produtos solicitados.
* 👤 **Perfil do Usuário**: Gerenciamento de dados cadastrais e preferências.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Linguagem**: [Kotlin](https://kotlinlang.org/)
* **Padrão de Arquitetura**: **MVVM (Model-View-ViewModel)** com separação clara de responsabilidades.
* **Injeção de Dependências**: **Dagger Hilt** para desacoplamento e facilidade de testes.
* **Componentes Android Jetpack**:
  * *Navigation Component* para fluxo entre fragments.
  * *ViewModel* & *LiveData* / *StateFlow* para controle de estado reativo.
  * *View Binding* para manipulação segura de layouts XML.
* **Backend as a Service (Firebase)**:
  * **Firebase Auth**: Gestão de identidade e sessões de usuários.
  * **Cloud Firestore**: Banco de dados NoSQL em tempo real para catálogo, pedidos e endereços.
  * **Firebase Storage**: Armazenamento de imagens e assets de produtos.
* **Carregamento de Imagens**: Glide para cache e renderização assíncrona.

---

## 📂 Estrutura do Código-Fonte

```
app/src/main/java/com/example/gaseagua/
├── data/           # Modelos de dados e entidades
├── di/             # Módulos de injeção de dependência (Hilt)
├── firebase/       # Integrações diretas e helpers do Firebase
├── fragments/      # Telas (Login, Home, Carrinho, Endereço, Perfil)
├── util/           # Extensões, validações e classes de apoio
└── viewmodel/      # ViewModels para gerenciamento de estado da UI
```

---

## 🚀 Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/aomaaj/Projeto-POO.git
   ```
2. Abra o projeto no **Android Studio** (versão Ladybug / Hedgehog ou superior recomendada).
3. **Configuração do Firebase**:
   * Crie um projeto no [Firebase Console](https://console.firebase.google.com/).
   * Baixe o arquivo `google-services.json` e adicione-o na pasta `app/` (consulte `app/google-services.json.example` como referência).
4. Aguarde a sincronização do Gradle e execute o app em um emulador ou dispositivo físico com Android 8.0 (API 26) ou superior.

---

## 👨‍💻 Autor

Desenvolvido por **João Mateus** ([@aomaaj](https://github.com/aomaaj)).
