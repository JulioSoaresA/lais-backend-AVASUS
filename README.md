# AVASUS-lais-backend
Repositório destinado ao armazenamento e versionamento do desafio/fase 2 da seleção para pesquisador no Projeto “PESQUISA APLICADA A IMPLEMENTAÇÃO DE PROCESSOS EDUCACIONAIS EM SISTEMAS INTEGRADOS DE INFORMAÇÃO E COMUNICAÇÃO EM SAÚDE”. Edital 021/2022 LAIS/HUOL/UFRN.

Candidato: Júlio César Almeida Soares

# Instalação
### Instalação de Ambiente Virtual
- Baixe esse repositório e Entre no diretório respectivo
- Utilize um VirtualEnvironment<br>
`python -m venv venv`


### Passos Iniciais para Funcionamento do Projeto
 - Crie e Execute de migrations para o banco de dados<br>
`python manage.py makemigrations`<br>
`python manage.py migrate`

- É necessário criar um SuperUsuário<br>
`python manage.py createsuperuser`
	- Dados necessários:
		- CPF Válido ( [Gerador de CPF](https://www.4devs.com.br/gerador_de_cpf) )
		- Data de Nascimento
		- Senha
    - Titulação (GRADUACAO, ESPECIALIZACAO, MESTRADO OU DOUTORADO)
    - Termos de uso (SIM ou NAO)

- Agora é so iniciar o servidor<br>
`python .manage.py runserver`

# Suporte de Avaliação
### História de Usuário #1 - Página Inicial *
 - [ ] CA#01 - Informações de Usuário Autenticado
 - [ ] CA#02 - Botão de encerrar sessão
 - [ ] CA#03 - Cadastro de novos planos de curso
 - [ ] CA#04 - Botões de Login e cadastre-se para Usuários não-autenticados

### História de Usuário #2 - AutoCadastro *
 - [x] CA#01 - Campos de formulário de autocadastro
 - [x] CA#02 - Validação de idade
 - [x] CA#03 - Validação de CPF
 - [x] CA#04 - CPF único
 - [x] CA#05 - Mensagem de confirmação ou negação

### História de Usuário #3 - Página de Login *
 - [x] CA#01 - Campos de login com CPF e senha
 - [x] CA#02 - Validação de campos
 - [x] CA#03 - Redirecionamento de login
 - [x] CA#04 - Utilização do Sistema de Autenticação Django(UserCreationForm)

### História de Usuário #4 - Administração da plataforma *
 - [ ] CA#01 - Command para inserir todas as áreas temáticas
 - [ ] CA#02 - Listagem dos objetos inseridos
 - [ ] CA#03 - Status do plano de curso
 
 ### História de Usuário #5 - Planos de Curso *
 - [ ] CA#01 - Listar cursos
 - [ ] CA#02 - Informações mais detalhadas dos cursos listados ao clicar
 - [ ] CA#03 - Botão de Cadastrar Tópicos de Aula
 - [ ] CA#04 - Botão de Submeter Novo Plano
 - [ ] CA#05 - Status de "Pendente de Aprovação"
 
 ### História de Usuário #6 - Tópicos de Aula *
 - [ ] CA#01 - Apenas planos de curso APROVADOS terão tópicos de aula cadastrados
 - [ ] CA#02 - Máximo de 5 tópicos permitidos
 - [ ] CA#03 - Informações do tópico
 - [ ] CA#04 - Descrição habilitada para formatação Markdown
 
 ### História de Usuário #7 - Certificado de Cursos Ministrados *
 - [ ] CA#01 - Botão para gerar certificado
 - [ ] CA#02 - Cabeçalho com nome e CPF do professor
 - [ ] CA#03 - Listagem de status
 - [ ] CA#04 - Código de unicidade
 - [ ] CA#05 - Exportar em PDF

## Não-Obrigatórias
### História de Usuário#8 - Validar o Certificado de Cursos Ministrados
 - [ ] CA#01 - Link para validação de certificado com 2 campos
 - [ ] CA#02 - Submissão do formulário apenas com os 2 campos preenchidos