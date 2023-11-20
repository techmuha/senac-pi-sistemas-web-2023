# senac-pi-sistemas-web-2023

# Sistema de Gestão Escolar
![1 0-login](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/d33a9b66-692c-42ce-8708-5bbd8234b0c7)

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
![0 0-fluxo](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/70ce4b91-63c6-40d8-ac33-287da85985ef)

## Descrição dos Cenários

![2 0-homepage](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/80726434-af53-4d15-9a8b-cf99d857b203)

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

   ![3 0-matriculas](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/e063ac29-0513-41d7-9bb0-d81ec1575915)
   ![3 1-matriculas-cadastro](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/a3316862-0979-471c-83a7-5a2f6d156a27)
   ![3 2-matriculas-detalhes](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/4508a7ae-40c0-46fd-80cc-0683e935dba5)
   ![3 3-matriculas-confirmacao](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/e60e4c09-c353-4344-bf67-b7dc4738923f)
  
- **Cenário Alternativo 1:**
  - *Passo 5:* Se os dados não forem válidos, o sistema exibe uma mensagem de erro e retorna ao passo 2.

- **Cenário Alternativo 2:**
  - *Passo 4:* O usuário pode cancelar o cadastro clicando no botão "Cancelar".

  ![4 3-pessoas-fisicas-confirmacao](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/800f6a1a-bd15-4483-88af-58dbb4a26902)


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

![5 0-pessoas-juridicas](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/16327750-6134-4edb-9ad9-382ecbec5d91)
![5 1-pessoas-juridicas-cadastro](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/22acb24a-fedf-4e20-a508-0b3cd0c22524)
![5 2-pessoas-juridicas-detalhes](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/95a78fc4-66fb-46f7-a395-b46c7ec695d2)
![5 3-pessoas-juridicas-confirmacao](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/6ca0afc5-f0ce-4d5d-8d8a-2f8cf668faac)

![4 0-pessoas-fisicas](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/3067dc66-c4ac-482c-81cb-6a173cd58f0d)
![4 1-pessoas-fisicas-cadastro](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/d018adf2-375d-42d9-80f2-98e8cb67f3fc)
![4 2-pessoas-fisicas-detalhes](https://github.com/techmuha/senac-pi-sistemas-web-2023/assets/151533400/a8236e51-ea7b-4f07-b5c1-9c8cd58f5bc0)


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
