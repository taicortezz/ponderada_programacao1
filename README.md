
Nome: Tainá Cortez.

# Template Readme para Arquitetura MVC em Markdown
- Nome do Projeto: Abandono 0
- Descrição: O projeto tem como foco compreender as causas por trás dos fenômenos de compra, adoção e/ou abandono de animais de estimação, com intenção de  reduzir o abandono. Através da coleta de dados sobre o comportamento dos tutores, é possivel compreender mais profundamente os motivos que levam a essas ações. Dessa forma, serão tomadas medidas para diminuir as causas do abandono.
- Arquitetura: MVC (Model-View-Controller)
- Ferramenta de Diagramação: draw.io
# Modelos (Models):

&nbsp;&nbsp;&nbsp;&nbsp; No projeto Abandono zero, por enquanto, existe apenas uma entidade chamada "users", que contém atributos para a identificação dos usuários. Esses atributos são: identificador único (id), endereço de e-mail (email) associado a cada conta, senha (senha) de cada e-mail e a função do usuário (role), que determina seus privilégios no sistema e é usado para distinguir entre administradores e usuários comuns. Além disso, há os modelos para armazenar as respostas de cada formulário e uma tabela de resultados visível apenas para o administrador.


# Controladores (Controllers):


&nbsp;&nbsp;&nbsp;&nbsp;"Controllers" é a camada responsável pelas interações do usuário na plataforma e  por ligar o model e a view, fazendo com que os models possam ser repassados para as views e vice-versa, direcionando o fluxo da aplicação. Os controllers desse projeto são:
- Verificar: Este controller valida o login do usuário, verificando se o login e senha estão corretos.
- Gravar: Responsável por salvar as respostas de todos os formulários preenchidos pelos usuários.
- Listar: Este controller permite listar as respostas dos formulários para visualização.
- Procurar: Oferece a funcionalidade de pesquisa para que o administrador possa encontrar as respostas com mais facilidade.

# Views (Views):

&nbsp;&nbsp;&nbsp;&nbsp;Até o momento, temos as seguintes telas:

- Tela inicial: Explica um pouco sobre o INSPA e o projeto Abandono Zero, além de ter as opções de cadastro ou login.
- Tela de cadastro: Solicita algumas informações do usuário para realizar o cadastro, como nome, sobrenome, telefone, endereço, email e senha.
- Tela de login: Solicita email e senha já cadastrados.
- Página inicial do formulário: Explica os objetivos da pesquisa e apresenta o botão para iniciar e selecionar as opções: "Já tive", "Tenho", "Quero ter" ou "Não quero ter" cachorro.
- Formulário "Já tive cachorro": Destinado a pessoas que já tiveram um cão no passado.
- Formulário "Tenho cachorro": Destinado a pessoas que têm um cachorro atualmente.
- Formulário "Quero ter cachorro": Para pessoas que planejam ter um cão no futuro.
- Formulário "Nulo": Para quem não quer ter um cachorro.
- Página do administrador: Onde o pesquisador tem acesso às respostas e dados dos formulários.

# Infraestrutura:
&nbsp;&nbsp;&nbsp;A infraestrutura do projeto baseia-se em um banco de dados gerenciado pelo sistema PostgreSQL, que é responsável por armazenar as respostas dos formulários de todos os usuários cadastrados na plataforma que participaram da pesquisa. Seguindo a arquitetura MVC (Model-View-Controller), o acesso e manipulação dos dados são realizados pela camada model, garantindo uma separação clara das responsabilidades e uma estrutura organizada.

# Justifique as escolhas feitas e como elas impactam o projeto.
Implicações da Arquitetura:
Descreva as implicações da arquitetura em termos de escalabilidade, manutenção, testabilidade e outros aspectos importantes.

&nbsp;&nbsp;&nbsp; A arquitetura MVC (Model-View-Controller) promove uma divisão estruturada do site em camadas, facilitando o entendimento e aprimoramento de suas funcionalidades. Essa estrutura é importante para a escalabilidade do projeto, pois permite modificações sem impactar no restante do site. Além disso, ao pensar em manutenção e testabilidade, a separação em camadas possibilita a realização de testes e correções de forma individualizada em cada parte do código, reduzindo assim a ocorrência de bugs e facilitando a manutenção contínua do sistema.

# Recursos Adicionais:
Documentação do Sails.js: https://github.com/balderdashy/sails Tutorial do draw.io: https://m.youtube.com/watch?v=w3zm-wbmlpc Exemplos de diagramas MVC: https://www.lucidchart.com/pages/templates

