# documenta-UCIA - Assistente Virtual da UNIGRAN

## Sobre o Projeto

O **UCIA (UNIGRAN Chatbot Inteligente de Atendimento)** é um assistente virtual desenvolvido para atender alunos, candidatos e interessados nos serviços acadêmicos da UNIGRAN.

O sistema tem como objetivo fornecer informações acadêmicas, institucionais e administrativas de forma rápida, clara e objetiva, facilitando a comunicação entre a comunidade acadêmica e a instituição.

A solução foi desenvolvida utilizando Python e Streamlit, com uma base de conhecimento estruturada em documentos Markdown contendo informações oficiais da universidade.

---

# Instituição de Ensino

## UNIGRAN - Centro Universitário da Grande Dourados

A UNIGRAN destaca-se como uma das principais instituições de ensino superior do Centro-Oeste brasileiro.

Com sede em Dourados-MS e forte atuação em Campo Grande-MS, oferece cursos nas modalidades:

* Presencial
* Educação a Distância (EAD)
* Pós-graduação

---

# Objetivos do UCIA

O assistente virtual foi desenvolvido para:

* Responder dúvidas frequentes de alunos e candidatos;
* Orientar processos de matrícula e ingresso;
* Disponibilizar informações institucionais oficiais;
* Facilitar o acesso aos serviços acadêmicos;
* Melhorar a comunicação entre estudantes e instituição;
* Apoiar o desenvolvimento acadêmico.

---

# Áreas de Formação

## Saúde

* Odontologia
* Medicina Veterinária
* Estética
* Psicologia

## Tecnologia

* Análise e Desenvolvimento de Sistemas

## Negócios e Humanas

* Direito
* Administração
* Pedagogia

## Agrárias e Engenharia

* Agronomia
* Engenharia Civil

---

# Saudação Inicial

```text
Olá! Sou UCIA, sua assistente virtual da UNIGRAN.

Estou pronta para ajudar com informações sobre cursos, vestibular, matrícula, bolsas, modalidades de ensino e demais serviços acadêmicos.

Como posso ajudar você hoje?
```

---

# Fluxo de Atendimento

## Menu Principal

### Cursos

* Graduação
* Pós-graduação
* Cursos Livres
* Extensão

### Modalidades

* Presencial
* Educação a Distância (EAD)

### Portal de Cursos

Informações detalhadas sobre cursos e grade curricular.

### Formas de Ingresso

* Vestibular Agendado
* Vestibular Online
* Nota do ENEM
* Segunda Graduação
* Transferência Externa

### Bolsas e Benefícios

* Bolsas de estudo
* Descontos institucionais
* Financiamentos estudantis

---

# Formas de Ingresso

## Vestibular

* Vestibular Agendado
* Vestibular Online

## ENEM

Ingresso utilizando a nota do Exame Nacional do Ensino Médio.

## Segunda Graduação

Ingresso para portadores de diploma de ensino superior.

## Transferência Externa

Transferência de alunos provenientes de outras instituições.

---

# Documentação Necessária para Matrícula

## Identificação

* RG
* CPF

## Escolaridade

* Histórico Escolar
* Certificado ou Certidão de Conclusão do Ensino Médio

## Documentação Civil

* Certidão de Nascimento ou Casamento

## Comprovante de Residência

* Atualizado

---

# Unidade Campo Grande

## Endereço

UNIGRAN – Centro Universitário

Rua Abrão Júlio Rahe, nº 325
Centro / Monte Castelo
Campo Grande – MS

CEP: 79010-010

## Telefone

(67) 3389-3389

---

# Canais Oficiais

## Site Oficial

https://www.unigran.br

## Atendimento Telefônico

(67) 3389-3389

## Ambiente Virtual

Plataforma Acadêmica UNIGRAN

---

# Principais Funcionalidades

## Atendimento Acadêmico

* Responder dúvidas frequentes;
* Orientar candidatos;
* Informar sobre cursos;
* Informar sobre modalidades de ensino;
* Orientar processos de ingresso.

## Comunicação Institucional

* Disponibilizar informações oficiais;
* Direcionar usuários aos setores responsáveis;
* Facilitar o contato com a instituição.

## Apoio ao Conhecimento

* Promover acesso à informação;
* Apoiar estudantes em sua jornada acadêmica;
* Facilitar a busca por conteúdos institucionais.

---

# Limitações do Assistente

O UCIA não realiza:

* Matrículas automáticas;
* Alterações cadastrais;
* Emissão de documentos oficiais;
* Processos administrativos internos;
* Decisões acadêmicas.

Nesses casos, o usuário deverá ser direcionado aos canais oficiais da instituição.

---

# Funcionamento do Sistema

O fluxo de funcionamento ocorre da seguinte forma:

1. O usuário acessa a aplicação.
2. Envia uma pergunta ao UCIA.
3. O sistema consulta a base de conhecimento.
4. As informações são processadas.
5. A resposta é gerada.
6. O resultado é apresentado ao usuário.

---

# Arquitetura do Sistema

```text
Usuário
   │
   ▼
Interface Streamlit
   │
   ▼
UCIA - Assistente Virtual
   │
   ├── Base de Conhecimento
   │      ├── Cursos
   │      ├── Modalidades
   │      ├── Vestibular
   │      ├── ENEM
   │      ├── Bolsas
   │      └── Matrícula
   │
   ├── Motor de Respostas
   │
   └── Integração com IA
   │
   ▼
Resposta ao Usuário
```

---

# Estrutura da Base de Conhecimento

A base de conhecimento contém documentos institucionais relacionados a:

* Cursos;
* Vestibular;
* ENEM;
* Bolsas;
* Matrícula;
* Transferências;
* Pós-graduação;
* Contatos;
* Informações institucionais.

---

# Estrutura de Pastas

```text
ucia/
│
├── app.py
│
├── docs/
│   ├── unigran.md
│   ├── cursos.md
│   ├── vestibular.md
│   ├── bolsas.md
│   └── matricula.md
│
├── data/
│   └── conhecimento.json
│
├── services/
│   ├── chatbot.py
│   ├── prompts.py
│   ├── knowledge.py
│   └── embeddings.py
│
├── utils/
│   ├── loader.py
│   └── formatter.py
│
├── assets/
│   ├── logo.png
│   └── imagens/
│
├── config/
│   └── settings.py
│
├── requirements.txt
├── .env
└── README.md
```

---

# Descrição dos Arquivos

## app.py

Arquivo principal responsável pela inicialização do Streamlit, interface do usuário e gerenciamento das interações.

## docs/

Armazena toda a documentação institucional utilizada como fonte de conhecimento.

## data/

Contém dados estruturados utilizados pela aplicação.

## services/

Implementa as regras de negócio.

### chatbot.py

Gerenciamento das conversas.

### prompts.py

Definição dos prompts do assistente.

### knowledge.py

Consulta e recuperação da base de conhecimento.

### embeddings.py

Processamento de informações para mecanismos de busca semântica e RAG.

## utils/

Funções auxiliares.

### loader.py

Carregamento dos documentos Markdown.

### formatter.py

Formatação das respostas.

## assets/

Arquivos estáticos como imagens, logos e ícones.

## config/

Configurações gerais do sistema.

### settings.py

Centralização de parâmetros e variáveis da aplicação.

---

# Tecnologias Utilizadas

| Tecnologia | Finalidade              |
| ---------- | ----------------------- |
| Python     | Linguagem principal     |
| Streamlit  | Interface Web           |
| Markdown   | Base de conhecimento    |
| OpenAI API | Inteligência Artificial |
| Ngrok      | Publicação local        |
| Git/GitHub | Controle de versão      |
| JSON       | Estruturação de dados   |

---

# Exemplo de Conversação

## Pergunta

Quais cursos de tecnologia a UNIGRAN oferece?

## Resposta

A área de Tecnologia da UNIGRAN oferece:

* Análise e Desenvolvimento de Sistemas

---

## Pergunta

Como posso ingressar na faculdade?

## Resposta

Você pode ingressar através de:

* Vestibular
* Nota do ENEM
* Segunda Graduação
* Transferência Externa

---

## Pergunta

Quais documentos preciso para matrícula?

## Resposta

Você precisará apresentar:

* RG
* CPF
* Histórico Escolar
* Certidão de Conclusão do Ensino Médio
* Certidão de Nascimento ou Casamento
* Comprovante de residência atualizado

---

# Benefícios da Arquitetura

* Organização modular;
* Fácil manutenção;
* Escalabilidade;
* Atualização rápida da base de conhecimento;
* Separação entre conteúdo, interface e lógica;
* Possibilidade de integração futura com sistemas acadêmicos;
* Suporte à implementação de RAG e banco vetorial.

---

# Informações do Projeto

| Campo       | Descrição          |
| ----------- | ------------------ |
| Nome        | UCIA               |
| Tipo        | Assistente Virtual |
| Instituição | UNIGRAN            |
| Unidade     | Campo Grande - MS  |
| Linguagem   | Python             |
| Framework   | Streamlit          |
| Publicação  | Ngrok              |

---

# Licença

Documento elaborado para fins acadêmicos, institucionais e de desenvolvimento do Assistente Virtual UCIA.
