**Desafio Técnico: Importação de Dados para o Solr**

**Descrição:**

Seu objetivo é criar um script em Python que realiza as seguintes tarefas:

1. **Formatar o CSV:**
   - O script deve ler um arquivo CSV fornecido e realizar a formatação dos dados para garantir consistência e correção.
   - Considere que o arquivo CSV pode conter campos mal formatados, dados ausentes ou outros problemas típicos em conjuntos de dados do mundo real.

2. **Inserir no Solr:**
   - Após a formatação, o script deve inserir os dados no Apache Solr. 
   - Certifique-se de mapear corretamente os campos do CSV para os campos correspondentes no esquema do Solr.

**Requisitos Técnicos:**

- Use a biblioteca `pandas` para manipulação de dados CSV em Python.
- Utilize a biblioteca `pysolr` para interagir com o Solr a partir do script Python.
- Hospede seu projeto no GitHub, fornecendo instruções claras sobre como configurar e executar o script.

**Configuração do Solr em Docker:**

Execute o seguinte comando para criar uma instância do Solr no Docker:

```bash
docker run -d -p 8983:8983 --name solr_instance -t solr
```

Acesse o Solr Admin Interface em http://localhost:8983/solr.

**Arquivo CSV de Exemplo (Alunos de uma Escola Primária):**

Utilize o arquivo [alunos.csv](https://github.com/joaomarcelo81/DesafioUBc/blob/main/aluno.csv) com os dados fictícios representando alunos de uma escola primária. 

**Pontos Extras:**

- Lidar com situações de erro durante a formatação e inserção no Solr.
- Implementar logs adequados para rastrear o progresso e eventuais problemas.
- Garantir que o script seja eficiente, mesmo para grandes conjuntos de dados.

**Instruções:**

1. Baixe o arquivo CSV de exemplo contendo dados fictícios de alunos de uma escola primária.
2. Desenvolva o script em Python.
3. Documente claramente como o script deve ser executado, incluindo dependências e configurações.
4. Hospede o projeto no GitHub e forneça o link do repositório.

**Avaliação:**

Você será avaliado com base na eficácia do script, na capacidade de lidar com situações não ideais nos dados e na integração bem-sucedida com o Solr. A utilização do GitHub para hospedar o projeto será considerada na avaliação global.
