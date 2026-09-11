# SyncHealth

O SyncHealth será um aplicativo de saúde móvel desenvolvido para reduzir o tempo de espera dos pacientes e melhorar o acesso às unidades de saúde pública. Os dados da fila em tempo real serão coletados dos usuários e exibidos em um mapa interativo. O agendamento de consultas será feito remotamente, para que os pacientes sejam notificados quando for a hora de se deslocarem até a unidade.

---

## Autora

- Leandra Lemos

---

## Tecnologias Usadas

- **JavaScript** — Principal linguagem de programação que será utilizada em toda a aplicação (lógica de front-end e back-end)
- **MySQL** — Será utilizado para armazenar e gerenciar todos os dados da aplicação (usuários, agendamentos, condições médicas, histórico)
- **Figma / Canva** — Serão utilizados para o design das telas da aplicação e materiais de apresentação
- **GitHub / VSCode** — Serão utilizados para controle de versão, colaboração em equipe e edição de código

---

## Funções

- As unidades de saúde próximas ao usuário serão exibidas em tempo real em um mapa interativo, com tempos de espera codificados por cores (rápido, médio, lento).

- Os agendamentos serão feitos remotamente, para que os pacientes só precisem se deslocar quando estiver próximo do seu atendimento.

- Um chatbot estará equipado com protocolos de triagem (como o Protocolo de Manchester) para que os pacientes sejam orientados e monitorados antes da chegada.

- Perfis de saúde familiar serão póssiveis, permitindo que os dependentes sejam gerenciados em uma única conta.

- Informações individuais sobre cada unidade (tipo, endereço, status) serão disponibilizadas aos pacientes diretamente no aplicativo.

- Um recurso de SOS estará incluído para que situações de emergência sejam sinalizadas imediatamente.

---

## Instalação

 Acesse o link e instale a aplicação. Após siga o passo a passo acéssivel de cadastro.

---

## Registro de alterações

### v1.0.0
- O esquema base do banco de dados (diagrama ER) foi projetado e modelado com todas as entidades principais: `usuario`, `atendimento`, `unidade_de_saude`, `familia`, `condicao_medica`, `medicacao` e `historico`.

- Os wireframes iniciais para a tela inicial, o menu lateral e a tela de login foram criados no Figma.

- O modelo relacional (lógico) foi mapeado a partir do diagrama ER e todas as chaves estrangeiras foram definidas.

---

## Problemas Conhecidos

- Não há problemas conhecidos no código até o momento, pois o desenvolvimento ainda não começou.

---

## A ser trabalhado

- Serão adicionadas notificações push para que os pacientes sejam alertados automaticamente quando sua posição na fila mudar.

- O chatbot do Protocolo de Manchester será totalmente integrado para que as recomendações de triagem sejam geradas automaticamente para cada sessão do paciente.

- Um sistema de feedback será implementado para que as avaliações e comentários dos pacientes sejam coletados após cada consulta.

- O modo escuro será adicionado em uma versão futura para melhorar a acessibilidade.

---

## Regras e Requisitos

- As respostas do chatbot devem ser revisadas por um profissional médico antes que o sistema seja disponibilizado ao público.

- O acesso ao perfil familiar deve ser restrito por regras de permissão, que ainda não foram totalmente implementadas.

- As senhas dos usuários devem ser criptografadas antes de serem armazenadas no banco de dados.

- Dados inválidos ou incompletos do formulário devem ser rejeitados pelo sistema antes que qualquer registro seja salvo.

- A posição na fila e o tempo de espera devem ser recalculados automaticamente sempre que um novo check-in for registrado.

- O acesso ao perfil familiar deve ser autorizado pelo titular da conta antes que os dados de qualquer dependente sejam visualizados ou editados.

- As solicitações de emergência (SOS) devem ser priorizadas e não devem ser bloqueadas por nenhuma restrição de fila ou agendamento.

- O histórico médico do paciente deve ser protegido e só pode ser acessado pelo titular da conta autenticado.

## Estrutura

SyncHealth
│
├── README.md
├── .gitignore
├── LICENSE
│
├── .github
│
├── docs
│
├── sql
│
└── src