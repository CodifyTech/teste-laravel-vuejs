# Teste para Desenvolvedor em Laravel e VueJS

## Requisitos do Projeto
- **Backend**: API em Laravel
- **Frontend**: SPA em VueJS
- **Funcionalidades**:
  - Login
  - Cadastro de Usuários
  - CRUD de Livros
  - CRUD de Autores
  - CRUD de Editoras

## Especificações Detalhadas

### Modelagem de Dados
- **Usuários**:
  - id (incremental, primary key)
  - nome (string)
  - email (string, único)
  - senha (string)
  - timestamps (created_at, updated_at)
  
- **Livros**:
  - id (incremental, primary key)
  - título (string)
  - descrição (text)
  - autor_id (foreign key para Autores)
  - editora_id (foreign key para Editoras)
  - publicado_em (date)
  - timestamps (created_at, updated_at)
  
- **Autores**:
  - id (incremental, primary key)
  - nome (string)
  - biografia (text)
  - data_nascimento (date)
  - timestamps (created_at, updated_at)
  
- **Editoras**:
  - id (incremental, primary key)
  - nome (string)
  - endereço (string)
  - telefone (string)
  - timestamps (created_at, updated_at)

### Backend (Laravel)
- Criar uma autenticação JWT para as rotas protegidas.
- Criar modelos, migrações e controladores para:
  - Usuários
  - Livros
  - Autores
  - Editoras
- Implementar as rotas de API:
  - Login (rota pública)
  - Cadastro de Usuários (rota pública)
  - CRUD para Livros (rotas protegidas)
  - CRUD para Autores (rotas protegidas)
  - CRUD para Editoras (rotas protegidas)
- Implementar validações de dados adequadas para todas as entradas.

### Frontend (VueJS)
- Configurar um novo projeto VueJS.
- Utilizar Vue Router para gerenciamento de rotas.
- Opcional:
  - Utilizar Pinia para gerenciamento de estado.
  - Utilizar Vuetify
- Criar componentes para:
  - Página de Login
  - Cadastro de Usuários
  - Listagem de Livros
  - Cadastro/Edição de Livros
  - Listagem de Autores
  - Cadastro/Edição de Autores
  - Listagem de Editoras
  - Cadastro/Edição de Editoras
- Consumir a API Laravel para cada uma das funcionalidades acima.
- Implementar autenticação no frontend e armazenamento do token JWT.

### Passos para Avaliação
1. **Desenvolvimento**:
   - Implementar as funcionalidades de backend e frontend conforme especificado.
   - Documentar os passos necessários para rodar o projeto.

2. **Entrega**:
   - Subir o código em um repositório público (GitHub, GitLab, etc.).
   - Fornecer instruções de instalação e execução do projeto.
   - Fornecer um breve vídeo (1 a 2 minutos) demonstrando as funcionalidades implementadas.

### Critérios de Avaliação
- **Qualidade do Código**: Organização, clareza e boas práticas.
- **Funcionalidade**: Completa implementação dos requisitos.

## Recursos
- Documentação do Laravel: [Laravel](https://laravel.com/docs)
- Documentação do VueJS: [VueJS](https://vuejs.org/v2/guide/)
- JWT Auth para Laravel: [jwt-auth](https://github.com/tymondesigns/jwt-auth)
- Vue Router: [Vue Router](https://router.vuejs.org/)
- Vuex: [Vuex](https://vuex.vuejs.org/)