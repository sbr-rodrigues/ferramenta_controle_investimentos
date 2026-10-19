# ferramenta_controle_investimentos
Este projeto foi desenvolvido como desafio da DIO (Digital Innovation One) com o objetivo de criar uma ferramenta em Excel capaz de simular investimentos em Fundos Imobiliários (FIIs).

#💸Simulador de Investimentos em Fundos Imobiliários (FIIs)
Descrição

###Este projeto foi desenvolvido como desafio da DIO (Digital Innovation One) com o objetivo de criar uma ferramenta em Excel capaz de simular investimentos em Fundos Imobiliários (FIIs).

###A planilha permite que o usuário informe valores básicos de investimento e receba projeções de patrimônio acumulado, rendimentos mensais estimados e distribuição sugerida dos aportes de acordo com o perfil de investidor selecionado.

##Objetivo da Ferramenta🎯

###A ferramenta responde às seguintes perguntas:

###Quanto investir por mês;
###Por quantos anos investir;
###Qual a taxa de rendimento mensal;
###Quanto patrimônio será acumulado ao final do período;
###Quanto poderá ser recebido em dividendos mensais.

###Além disso, a planilha realiza projeções para diferentes horizontes de investimento e sugere uma distribuição do aporte entre diferentes categorias de FIIs.

##Funcionalidades
###Simulação de Investimentos

##A ferramenta permite configurar:

###Valor do aporte mensal;
###Prazo do investimento;
###Taxa de rendimento mensal;
###Perfil do investidor.

##Com base nesses dados, a planilha calcula automaticamente:

###Patrimônio acumulado;
###Dividendos mensais estimados;
###Cenários futuros de investimento.
###Projeção de Cenários

##📅Foram criadas simulações para:

###2 anos
###5 anos
###10 anos
###20 anos
###30 anos

###Os valores são atualizados automaticamente conforme os parâmetros informados pelo usuário.

##🧐Perfis de Investidor

###A planilha possui seleção de perfil através de lista suspensa.

##Perfis disponíveis:

###Conservador
###Moderado
###Agressivo

###Cada perfil possui uma distribuição específica entre os diferentes tipos de Fundos Imobiliários.

##Categorias de FIIs Utilizadas

###A distribuição dos aportes considera os seguintes tipos de fundos:

###Papel
###Tijolo
###Híbrido
###FOF's (Fund of Funds)
###Desenvolvimento
###Hotelaria
###Funções Utilizadas
###VF (Valor Futuro)

##A função VF foi utilizada para calcular o patrimônio acumulado considerando:

###Taxa de rendimento mensal;
###Quantidade de períodos;
###Aporte mensal.

###Essa função permite estimar quanto o investimento poderá valer ao final do prazo escolhido.

###Exemplo de aplicação:

=VF(taxa_mensal; prazo_em_meses; -aporte)

###PROCV

###A função PROCV foi utilizada para buscar automaticamente o percentual correspondente a cada categoria de FII de acordo com o perfil selecionado.

###Exemplo:

=PROCV(chave; tabela_apoio; 4; FALSO)

###Utilização de Chave Composta

Para localizar corretamente os percentuais de cada perfil foi criada uma chave composta utilizando:

##Perfil + Tipo de Fundo


###Exemplos:

###Conservador-Papel
###Conservador-Tijolo
###Moderado-Híbrido
###Agressivo-Papel


###Essa chave permite que o PROCV identifique exatamente qual percentual deve ser retornado para cada combinação de perfil e categoria de fundo.

##Intervalos Nomeados

###Foram utilizados intervalos nomeados para melhorar a organização e a legibilidade das fórmulas.

###Exemplos:

###aporte
###taxa_mensal
###salario
###prazo

###O uso de nomes facilita a manutenção da planilha e torna as fórmulas mais intuitivas.

##Estrutura do Projeto
###Aba Principal

###Responsável pela interação com o usuário, contendo:

###Entradas de dados;
###Simulações;
###Resultados;
###Distribuição dos investimentos.
###Aba de Apoio

##Responsável por armazenar:

###Tabela de perfis;
###Chaves compostas;
###Percentuais de distribuição;
###Dados utilizados pelo PROCV.
###Melhorias Implementadas

###Além dos requisitos do desafio, foram realizadas melhorias visuais para proporcionar uma experiência semelhante a um aplicativo:

###Layout organizado;
###Banner personalizado;
###Separação visual entre entrada de dados e resultados;
###Utilização de cores para facilitar a leitura.
###Tecnologias Utilizadas
###Microsoft Excel
###Fórmulas financeiras
###PROCV
###Validação de Dados
###Intervalos Nomeados
###Formatação Condicional
###Evidências
##Perfil Conservador🧐

images/conservador.png

##Perfil Moderado

images/moderado.png

##Perfil Agressivo

images/agressivo.png

##Conclusão

###Este projeto demonstra a aplicação de conceitos de Excel voltados para análise financeira, projeção de investimentos e automação de cálculos através de funções e tabelas de apoio.

###A solução foi construída com foco na experiência do usuário, possibilitando que qualquer pessoa realize simulações de investimento sem a necessidade de conhecer fórmulas ou conceitos avançados do Excel.
