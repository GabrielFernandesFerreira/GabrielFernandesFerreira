Aluno: Gabriel Fernandes Ferreira de Souza
RA: 116995-22

Controle Detalhado de Gastos - Elaboração Detalhada

O Controle Detalhado de Gastos é uma aplicação que viabiliza aos utilizadores administrar as suas despesas e liquidações de maneira bem-organizada. Através de uma interface em forma de texto, o utilizador pode interagir com diversas funcionalidades providenciadas pelo sistema para gerir as suas finanças pessoais.

Categorias:

Despesa (Categoria Base):

A categoria abstrata Despesa serve como base para todos os tipos de gastos. Contém características como descrição, quantia, data de vencimento e estado de pagamento. Adicionalmente, esta categoria detém funções como efetuar pagamento (para assinalar uma despesa como paga), listar detalhes (para apresentar informações da despesa) e obterCategoria (uma função abstrata para obter a categoria da despesa).
Alimentação e Transporte (Subcategorias de Despesa):

Alimentação e Transporte representam subcategorias da categoria Despesa. Ambas herdam características e funções da categoria principal e implementam a função abstrata obterCategoria. Cada uma destas subcategorias representa um tipo específico de gasto (alimentação e transporte, respetivamente).
Pagável (Interface):

A interface Pagável estabelece o acordo para objetos que podem ser alvo de pagamento. Exige a implementação da função registarPagamento, permitindo o registo de um pagamento para uma despesa pendente.
Utilizador:

A categoria Utilizador representa os utilizadores do sistema. Cada utilizador possui um nome de utilizador e uma palavra-passe. A categoria detém funções como verificarPalavraPasse (para comparar palavras-passe) e um construtor para criar novos utilizadores.
GestorDespesas:

A categoria GestorDespesas é responsável por administrar as despesas registadas no sistema. Mantém uma lista de despesas, possibilitando a adição de novas despesas através da função adicionarDespesa e a listagem de todas as despesas através da função listarDespesas.
TipoDespesa:

A categoria TipoDespesa é usada para formar categorias de despesa. Possui uma característica denominada nome que define o tipo de categoria. Esta categoria é utilizada na gestão de tipos de despesa.
Funções e Características:

Construtores Sobrepostos:

As categorias Alimentação e Transporte têm construtores sobrepostos que permitem a criação de instâncias destas categorias com diversos detalhes, como descrição, quantia e data de vencimento.
Registrar Pagamento:

A interface Pagável define a função registarPagamento, implementada na categoria Transporte. Permite ao utilizador registar o pagamento de uma despesa pendente, marcando-a como paga.
Listagem de Despesas por Intervalo de Tempo:

A função listarDespesasPorPeriodo recebe uma lista de despesas e um intervalo de datas. Filtra e retorna exclusivamente as despesas enquadradas no intervalo especificado.
Listagem de Despesas Pagas e Pendentes por Intervalo de Tempo:

As funções listarDespesasPagasNoPeriodo e listarDespesasEmAbertoNoPeriodo operam de modo similar à função anterior, mas retornam apenas despesas pagas ou pendentes dentro do intervalo especificado.
Gestão de Tipos de Despesa:

A categoria TipoDespesa possui uma característica denominada nome que define o tipo de despesa. Isso contribui para a organização e classificação dos gastos.
Gestão de Utilizadores:

A categoria Utilizador possibilita a inscrição, verificação de palavras-passe e autenticação dos utilizadores no sistema. Também simula a encriptação de palavras-passe para garantir a segurança.
Considerações Finais:

O Controle Detalhado de Gastos permite ao utilizador adicionar gastos, listar, filtrar e registar pagamentos. A implementação recorre a conceitos de hereditariedade, interfaces e polimorfismo para criar uma estrutura modular e reutilizável. Cada funcionalidade é representada por categorias e funções específicas, garantindo a organização e eficácia do sistema. Contudo, é crucial recordar que isto é apenas um exemplo elementar, e um sistema real exige ponderações adicionais, como segurança, usabilidade e persistência de dados.
