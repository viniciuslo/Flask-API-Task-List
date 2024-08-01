## Descrição do Projeto

Este projeto foi desenvolvido com o objetivo de estudar a implementação de operações CRUD (Create, Read, Update, Delete) utilizando o framework Flask em Python. Além disso, o projeto inclui a criação de testes automatizados utilizando a biblioteca Pytest.

## Estrutura do Projeto

- **app.py**: Arquivo principal que contém a implementação das rotas e lógica do servidor Flask.
- **models/task.py**: Arquivo que define a classe `Task`, representando uma tarefa no sistema.
- **tests/**: Diretório contendo os testes automatizados escritos com Pytest.

## Funcionalidades

### Rotas Implementadas

1. **POST /tasks**: Cria uma nova tarefa.
2. **GET /tasks**: Retorna a lista de todas as tarefas.
3. **GET /tasks/<int:id>**: Retorna uma tarefa específica pelo ID.
4. **PUT /tasks/<int:id>**: Atualiza uma tarefa específica pelo ID.
5. **DELETE /tasks/<int:id>**: Deleta uma tarefa específica pelo ID.

### Modelo de Dados

A classe `Task` possui os seguintes atributos:
- `id` : Identificador único da tarefa.
- `title` : Título da tarefa.
- `description`: Descrição da tarefa.
- `completed`: Status de conclusão da tarefa (padrão é `False`).

## Testes Automatizados

Os testes foram escritos utilizando a biblioteca Pytest. Eles cobrem as seguintes funcionalidades:
- Criação de tarefas.
- Recuperação de todas as tarefas.
- Recuperação de uma tarefa específica.
- Atualização de uma tarefa.
- Exclusão de uma tarefa.

### Executando os Testes

Para executar os testes, siga os passos abaixo:

1. Instale as dependências necessárias:
    ```bash
    pip install flask pytest
    ```

2. Execute os testes:
    ```bash
    pytest
    ```

## Como Executar o Projeto

1. Instale as dependências necessárias:
    ```bash
    pip install flask
    ```

2. Execute o servidor Flask:
    ```bash
    python app.py
    ```

3. O servidor estará disponível em `http://127.0.0.1:5000/`.

## Conclusão

Este projeto serviu como uma excelente oportunidade para praticar a implementação de operações CRUD utilizando Flask e a criação de testes automatizados com Pytest. Através deste estudo, foi possível compreender melhor a estrutura de um projeto Flask e a importância dos testes para garantir a qualidade do código.