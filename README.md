# Projeto Flutter: Uso de SharedPreferences

## Descrição do Projeto

Este projeto Flutter é um exemplo de como utilizar o plugin `shared_preferences` para armazenar dados simples localmente no dispositivo. O `shared_preferences` permite que você armazene e recupere dados em um formato chave-valor, semelhante ao armazenamento local em navegadores web.

## Objetivo

O objetivo deste projeto é demonstrar como:

- Configurar e utilizar o plugin `shared_preferences` em um aplicativo Flutter.
- Armazenar e recuperar dados de preferências do usuário, como nome de usuário, tema preferido, e configurações de notificação.
- Implementar uma interface simples onde o usuário pode visualizar e alterar suas preferências.

## Funcionalidades

1. **Armazenamento de Preferências do Usuário**
   - Salvar e recuperar o nome de usuário.
   - Salvar e recuperar preferências de tema (claro/escuro).
   - Salvar e recuperar configurações de notificação (ativadas/desativadas).

2. **Interface do Usuário**
   - Tela inicial que exibe as preferências atuais do usuário.
   - Tela de configurações onde o usuário pode alterar suas preferências.

3. **Persistência de Dados**
   - Garantir que as preferências do usuário sejam persistentes entre sessões do aplicativo.

## Estrutura do Projeto

- **`main.dart`**: Ponto de entrada do aplicativo que configura o MaterialApp e define a rota inicial.
- **`home_screen.dart`**: Tela inicial que exibe as preferências atuais do usuário.
- **`settings_screen.dart`**: Tela de configurações onde o usuário pode alterar suas preferências.
- **`storage_service.dart`**: Serviço responsável por ler e escrever dados usando o `shared_preferences`.

## Uso de `shared_preferences`

- **Salvar Dados**: Quando o usuário altera suas preferências na tela de configurações, os dados são salvos localmente usando `shared_preferences`.
- **Recuperar Dados**: Na inicialização do aplicativo e ao navegar para a tela inicial, os dados salvos são recuperados e exibidos ao usuário.

## Benefícios

- **Persistência Simples**: `shared_preferences` oferece uma maneira fácil de armazenar dados simples sem a necessidade de configurar um banco de dados completo.
- **Desempenho**: Operações de leitura e escrita são rápidas, o que proporciona uma experiência de usuário suave.
- **Simplicidade**: O uso do plugin é direto, facilitando a implementação mesmo para desenvolvedores iniciantes.

## Possíveis Extensões

- **Autenticação**: Integrar com um serviço de autenticação para salvar preferências personalizadas para cada usuário.
- **Sincronização na Nuvem**: Sincronizar preferências com um serviço de backend para persistência entre dispositivos.
- **Mais Preferências**: Adicionar mais opções de configuração, como idioma preferido, tamanho da fonte, etc.

Este projeto serve como uma base sólida para entender e implementar o armazenamento de preferências do usuário em um aplicativo Flutter, facilitando o desenvolvimento de aplicativos mais complexos no futuro.