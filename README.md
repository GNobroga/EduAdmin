# EduAdmin 

Este é um projeto simples desenvolvido para o desafio ZDZCode. Ele permite realizar operações de CRUD (Criar, Ler, Atualizar e Deletar) em um contexto educacional, facilitando a gestão de dados estudantis.

## Como usar

### Frontend 

Clone ou baixe os arquivos do repositório. Em seguida, siga os passos abaixo para configurar e executar o frontend:

1. Navegue até a pasta do frontend:

```bash
   cd frontend
```

2. Instale as dependências:
   
```bash
  npm install
```

3. Execute o projeto:

```bash
  npm run dev
```

### Backend

Clone ou baixe os arquivos do repositório. Em seguida, siga os passos abaixo para configurar e executar o backend:

1. Navegue até a pasta do backend:

```bash
   cd backend
```

2. Execute o projeto:

```bash
  dotnet run 
```

Certifique-se de ter o SDK do .NET na versão 8.0 instalado em seu sistema.

## Modelo Lógico

Este modelo tem como objetivo descrever a estrutura lógica do banco de dados.

- Users - Usuários
- Grades - Notas
- Classes - Salas
- Attendances - Chamadas
- Subjects - Disciplinas

![](/docs/diagrama.png)


## Telas

Todas as telas permitem realizar CRUD, consulta e algumas possuem funcionalidades a mais.

### Inicial 

![alt text](/docs/inicial.png)

### Estudante

#### Visualizar

![alt text](/docs/visualizar-estudante.png)


#### Criar

![alt text](/docs/criar-estudante.png)


#### Editar

![alt text](/docs/editar-estudante.png)

#### Deletar

![alt text](/docs/deletar-estudante.png)

#### Ver Notas

![alt text](/docs/ver-notas-estudante.png)

### Disciplinas

#### Visualizar

![alt text](/docs/visualizar-disciplinas.png)

#### Buscar

![alt text](/docs/buscar-disciplina-por-professor.png)

## API Endpoints

### Presença

#### Obter Contagem de Presenças por ID de Aluno

. GET `/student/{id:int}/count`


####  Obter Todas as Presenças

. GET `/`

#### Obter Presença por ID

. GET `/{id:int}`

#### Criar Presença

. POST `/`

#### Deletar Presença

. DELETE `/{id:int}`

#### Pesquisar por Presenças

. GET `/search?term=content`

### Classes

####  Obter Todas as Salas

. GET `/`

#### Obter Sala por ID

. GET `/{id:int}`

#### Criar Sala

. POST `/`

#### Deletar Sala

. DELETE `/{id:int}`

#### Pesquisar por Sala

. GET `/search?term=content`


### Notas

####  Obter Todas as Notas

. GET `/`

#### Obter Nota por ID

. GET `/{id:int}`

#### Criar Nota

. POST `/`

#### Deletar Nota

. DELETE `/{id:int}`

#### Pesquisar por Nota

. GET `/search?term=content`

#### Obter Notas por ID de Aluno

. GET `/student/{id:int}`

#### Obter Média de Notas por ID do Aluno

. GET `/student/{id:int}/average`


### Disciplinas

####  Obter Todas as Disciplinas

. GET `/`

#### Obter Disciplina por ID

. GET `/{id:int}`

#### Criar Disciplina

. POST `/`

#### Deletar Disciplina

. DELETE `/{id:int}`

#### Pesquisar por Disciplina

. GET `/search?term=content`

#### Obter Disciplinas por ID do professor

. GET `/teacher/{id:int}`

### Usuários

####  Obter Todas as Usuários

. GET `/`

#### Obter Usuário por ID

. GET `/{id:int}`

#### Criar Usuário

. POST `/`

#### Deletar Usuário

. DELETE `/{id:int}`

#### Pesquisar por Usuário

. GET `/search?term=content`


## Tecnologias

- Vue

- Nuxt

- Tailwind CSS

- C#

- ASP NET
