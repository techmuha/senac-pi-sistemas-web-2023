# senac-pi-sistemas-web-2023

# Sistema de Gestão Escolar
![1 0-login](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/863ca32c-1ec3-463a-868b-901493d7fb36)

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
![0 0-fluxo](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/fabb6604-5416-4f8f-bdf0-5e3283ce8484)

## Descrição dos Cenários

![2 0-homepage](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/da52247b-cac7-4682-8379-e3f245ae2a44)



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
   
   ![3 0-matriculas](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/c1a85d62-aa60-4bb0-855c-b5cb0be5f9d7)
  
   ![3 1-matriculas-cadastro](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/8f4a0fc1-2f69-4aa5-9d7d-22d781a9c4e3)
  
   ![3 2-matriculas-detalhes](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/bb04162c-1e70-48c5-a0d3-29a62c71438a)
  
   ![3 3-matriculas-confirmacao](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/849ef1d9-2f76-4484-a54a-9a3c64ac1cb3)
  
- **Cenário Alternativo 1:**
  - *Passo 5:* Se os dados não forem válidos, o sistema exibe uma mensagem de erro e retorna ao passo 2.

- **Cenário Alternativo 2:**
  - *Passo 4:* O usuário pode cancelar o cadastro clicando no botão "Cancelar".

  ![4 3-pessoas-fisicas-confirmacao](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/ea7a097c-ca7e-44cc-8183-3e2fa6c77ba6)

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
![5 0-pessoas-juridicas](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/a3cc38aa-8b67-4ea5-9629-73a569378cad)

![5 1-pessoas-juridicas-cadastro](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/440cf34f-9c5f-4520-b44b-6d6063d9e6fc)

![5 2-pessoas-juridicas-detalhes](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/4ff7f55b-e96c-4bc8-ab23-ebefe8a35bd4)

![5 3-pessoas-juridicas-confirmacao](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/3930e0b9-f7b0-49ef-8a8a-2369676e7905)

![4 0-pessoas-fisicas](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/6031509a-d067-404d-8711-1b665a774d5b)

![4 1-pessoas-fisicas-cadastro](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/b7b49a5e-c0b1-457d-b50c-5632be32e0eb)

![4 2-pessoas-fisicas-detalhes](https://github.com/cmpsleo/senac-pi-sistemas-web-2023/assets/144066589/0d6e4b3d-f89a-48ad-b1dd-162be6b653cc)

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
