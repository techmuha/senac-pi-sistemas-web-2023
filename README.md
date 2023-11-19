# senac-pi-sistemas-web-2023

# Sistema de Gestão Escolar
----Markdown Aplicativo de gestão escolar.----


## Diagrama de Casos de Uso

### Atores

1. Pessoa Física
2. Pessoa Jurídica
3. Professores
4. Fornecedores
5. Alunos

### Casos de Uso

1. Cadastrar Pessoa Física
2. Cadastrar Pessoa Jurídica
3. Cadastrar Professor
4. Cadastrar Fornecedor
5. Cadastrar Aluno
6. Consultar Dados de Pessoa Física
7. Consultar Dados de Pessoa Jurídica
8. Consultar Dados de Professor
9. Consultar Dados de Fornecedor
10. Consultar Dados de Aluno

## Diagrama de Casos de Uso
(Insira aqui a representação gráfica do diagrama de casos de uso)

## Descrição dos Cenários

### Cadastrar Pessoa Física

- **Cenário Principal:**
  - *Pré-condição:* O usuário tem permissão para cadastrar pessoas físicas.
  - *Pós-condição:* Uma pessoa física é cadastrada com sucesso no sistema.
  - *Fluxo de Eventos:*
    1. O usuário seleciona a opção "Cadastrar Pessoa Física".
    2. O sistema exibe o formulário de cadastro.
    3. O usuário preenche os campos obrigatórios, como nome, CPF, data de nascimento, etc.
    4. O usuário clica no botão "Salvar".
    5. O sistema valida os dados e cadastra a pessoa física.
    6. O sistema exibe uma mensagem de confirmação.

- **Cenário Alternativo 1:**
  - *Passo 5:* Se os dados não forem válidos, o sistema exibe uma mensagem de erro e retorna ao passo 2.

- **Cenário Alternativo 2:**
  - *Passo 4:* O usuário pode cancelar o cadastro clicando no botão "Cancelar".

### Consultar Dados de Professor

- **Cenário Principal:**
  - *Pré-condição:* O usuário está autenticado no sistema.
  - *Pós-condição:* Os dados do professor são exibidos.
  - *Fluxo de Eventos:*
    1. O usuário seleciona a opção "Consultar Dados de Professor".
    2. O sistema exibe uma lista de professores cadastrados.
    3. O usuário seleciona um professor da lista.
    4. O sistema exibe os detalhes do professor, como nome, disciplinas, etc.

- **Cenário Alternativo 1:**
  - *Passo 3:* Se não houver professores cadastrados, o sistema exibe uma mensagem informando que não há dados disponíveis.

## Diagrama de Classe

### Exemplo Simplificado do Diagrama de Classe

- **Classe Pessoa (Superclasse abstrata)**
  - *Atributos:* nome, CPF/CNPJ, data de nascimento, endereço, etc.

- **Classe PessoaFisica (Subclasse de Pessoa)**
  - *Atributos adicionais:* RG, gênero, estado civil, etc.

- **Classe PessoaJuridica (Subclasse de Pessoa)**
  - *Atributos adicionais:* Razão Social, CNPJ, representante legal, etc.

- **Classe Professor**
  - *Atributos:* disciplinas, formação, carga horária, etc.

- **Classe Aluno**
  - *Atributos:* matrícula, curso, período, etc.
