# SISTEMA INTELIGENTE PARA PREDIÇÃO DO DESEMPENHO ESTUDANTIL A PARTIR DE FATORES ACADÊMICOS, SOCIOECONÔMICOS E COMPORTAMENTAIS

**Daví Duarte, 1659455@pucminas.edu.br**

**Laura de Castro e Costa, 1674113@pucminas.edu.br**

**Guilherme Maurício de Souza Neves, 721950@pucminas.edu.br**

**Leticia Soares de Paiva Lacerda, leticia.lacerda.1451552@sga.pucminas.br**

**Leonardo Rodrigues dos Anjos Correa, 1412021@pucminas.edu.br**


---

Professores:

**Gabriel Barbosa da Fonseca**

---

_Curso de Ciência de Dados, Unidade Lourdes_

_Instituto de Informática e Ciências Exatas – Pontifícia Universidade de Minas Gerais (PUC MINAS), Belo Horizonte – MG – Brasil_

---

**Resumo**. Escrever aqui o resumo. O resumo deve contextualizar rapidamente o trabalho, descrever seu objetivo e, ao final, mostrar algum resultado relevante do trabalho (até 10 linhas)._

---

## Introdução

O desempenho acadêmico é um dos principais indicadores de qualidade da educação e está associado a trajetórias de trabalho, renda e cidadania. Contudo, a aprendizagem não depende apenas do tempo em sala de aula: hábitos de estudo, frequência, envolvimento familiar, condições socioeconômicas e características da escola se combinam de forma complexa. Este trabalho se insere nesse debate a partir da Ciência de Dados, com o propósito de transformar registros estudantis em evidências interpretáveis para apoiar decisões pedagógicas.
Utiliza-se a base Student Performance Factors, publicada no Kaggle, com 6.607 registros e 20 atributos sobre rotina de estudo, frequência, recursos educacionais, renda familiar, qualidade docente e nota final de exame. A pergunta que orienta o projeto é: quais fatores individuais, familiares e escolares, registrados nessa base, melhor explicam e predizem a nota de exame dos estudantes? A resposta será buscada por meio da preparação dos dados, da modelagem com ao menos dois algoritmos de aprendizado e da análise comparativa dos resultados.

###    Contextualização

A Agenda 2030 da Organização das Nações Unidas reconhece a educação de qualidade, inclusiva e equitativa como objetivo de desenvolvimento sustentável, o ODS 4. Na prática, esse compromisso se traduz em um desafio mensurável: garantir não apenas o acesso à escola, mas a aprendizagem efetiva. O desempenho em avaliações passou, portanto, a ser lido como síntese de múltiplos fatores — individuais, familiares e institucionais — e não como um atributo isolado do estudante.
O conjunto descreve, para cada estudante, variáveis numéricas (horas de estudo semanais, percentual de frequência, horas de sono, notas anteriores, sessões de tutoria, atividade física) e categóricas (envolvimento parental, acesso a recursos, motivação, acesso à internet, renda familiar, qualidade docente, tipo de escola, influência dos pares, deficiência de aprendizagem, escolaridade dos pais, distância casa-escola e gênero), tendo como variável-alvo a nota final de exame.

###    Problema

O problema abordado é a dificuldade de identificar, de modo sistemático e quantitativo, quais fatores mais se associam à nota de exame de um estudante quando várias dimensões atuam ao mesmo tempo. Na rotina escolar, decisões de reforço, recuperação e acompanhamento costumam apoiar-se em indicadores isolados — nota anterior, faltas ou percepção do professor — sem um modelo que articule hábitos de estudo, contexto familiar e características da escola.
Essa lacuna tem consequências práticas. Intervenções genéricas (por exemplo, aumentar o volume de conteúdo para toda a turma) podem ignorar que parte da variação do desempenho esteja ligada à frequência, à ausência de tutoria, à baixa motivação ou à falta de recursos em casa. Sem uma leitura multivariada, gestores e professores tendem a tratar sintomas (a nota baixa) sem distinguir causas mais próximas, como horas de estudo e assiduidade, de restrições estruturais, como renda familiar e qualidade docente.
O contexto de uso pretendido é o de apoio à decisão pedagógica e educacional, e não o de substituição do julgamento docente. A base escolhida não é um censo brasileiro: trata-se de um conjunto público, delimitado e já estruturado, com cerca de 6,6 mil registros. O problema, portanto, não é “melhorar a educação nacional” de forma abstrata; é estimar a nota de exame e ranquear os fatores associados a ela, a partir dos atributos disponíveis, de modo que as evidências possam informar políticas de frequência, tutoria e acompanhamento em ambientes escolares semelhantes.

###    Objetivo geral

Desenvolver um sistema inteligente capaz de prever a nota final de exame de estudantes a partir dos atributos acadêmicos, socioeconômicos e comportamentais da base Student Performance Factors, identificando quais fatores melhor explicam o desempenho.
Em formulação de pergunta orientada a dados: quais variáveis individuais, familiares e escolares da base Student Performance Factors melhor predizem a nota de exame, e com que grau de acerto dois algoritmos de aprendizado distintos conseguem estimar esse resultado?

####    Objetivos específicos

Apresente também alguns (pelo menos 2) **objetivos específicos** dependendo de onde 
você vai querer concentrar a sua prática investigativa, ou como você vai aprofundar 
no seu trabalho.

> **Links Úteis**:
> - [Objetivo geral e objetivo específico: como fazer e quais verbos utilizar](https://blog.mettzer.com/diferenca-entre-objetivo-geral-e-objetivo-especifico/)


###    Justificativas

A primeira justificativa é social e educacional. Um sistema que ajude a antecipar notas e a evidenciar fatores associados ao resultado pode apoiar ações mais precoces de frequência, reforço e tutoria, em linha com o ODS 4.
A segunda justificativa é de contribuição. O trabalho não pretende criar uma política pública nacional a partir de dados do Kaggle. A contribuição esperada é um pipeline reproduzível de Ciência de Dados aplicado a desempenho estudantil, com diagnóstico dos fatores mais associados à nota e com discussão honesta das limitações.

##    Público alvo


## 1. Perfis de Usuários

* *Gestores Escolaares (Diretores e Coordenadores):* Focam na parte estratégica e tomam decisões importantes. Precisam de painéis visuais para gerenciar recursos, planejar turmas de reforço e direcionar investimentos. Têm boa familiaridade com tecnologia.
* *Corpo Docente (Professores):* Usuários do dia a dia na sala de aula. Utilizam os alertas do sistema para identificar alunos que precisam de atenção e evitar a queda de desempenho. O nível de facilidade com ferramentas digitais varia bastante entre eles.
* *Equipe de Apoio (Orientadores e Psicólogos):* Focam no acolhimento e no suporte direto. Usam os dados socioeconômicos e de comportamento para planejar conversas e atendimentos focados com os estudantes e suas famílias.

---

## 2. Mapa de Stakeholders

### Alta Influência / Alto Interesse (Gerenciar de perto)
* Coordenadores Pedagógicos
* Diretores Escolares
* Professores (Corpo Docente)

### Baixa Influência / Alto Interesse (Manter informados)
* Alunos
* Pais e Responsáveis

### Alta Influência / Baixo Interesse (Manter satisfeitos)
* Equipe Técnica / TI da Escola
* Secretarias de Educação

### Baixa Influência / Baixo Interesse (Monitorar)
* Comunidade Escolar Geral
* Provedores de Dados (Kaggle)


## Análise exploratórida dos dados

###    Dicionário de dados

Apresente uma descrição das bases de dados a serem utilizadas. 
Dicionários de dados devem conter as bases de dados, os nomes dos atributos 
com seu significado, seu tipo (inteiro, real, textual, categórico, etc).

Este projeto deve utilizar pelo menos duas fontes de dados. Uma fonte principal e 
uma fonte para enriquecimentos dos dados principais.


###    Descrição de dados

Utilize a análise descritiva baseada em estatística de primeira ordem para descrever os dados.
Como descrever dados numéricos: média, desvio padrão, mínimo, máximo, quartis, histograma, etc.
Como descrever dados qualitativos (categóricos): moda (valor mais frequente), quantidade de valores distintos (categorias), distribuição das categorias (histograma), etc.


## Preparação dos dados

A preparação dos dados consiste dos seguintes passos:

> - Seleção dos atributos
> - Tratamentos dos valores faltantes ou omissos: remoção, substituição, indução, etc.
> - Tratamento dos valores inconsistentes: conversão, remoção de dados duplicados, remoção ou tratamento de ouliers.
> - Conversão de dados: p. ex. numérico para categórico, categórico para binário, etc.


## Indução de modelos

### Modelo 1: Algoritmo

Substitua o título pelo nome do algoritmo que será utilizado. P. ex. árvore de decisão, rede neural, SVM, etc.
Justifique a escolha do modelo.
Apresente o processo utilizado para amostragem de dados (particionamento, cross-validation).
Descreva os parâmetros utilizados. 
Apresente trechos do código utilizado comentados. Se utilizou alguma ferramenta gráfica, apresente imagens
com o fluxo de processamento.

### Modelo 2: Algoritmo

Repita os passos anteriores para o segundo modelo.


## Resultados

### Resultados obtidos com o modelo 1.

Apresente aqui os resultados obtidos com a indução do modelo 1. 
Apresente uma matriz de confusão quando pertinente. Apresente as medidas de performance
apropriadas para o seu problema. 
Por exemplo, no caso de classificação: precisão, revocação, F-measure, acurácia.

### Interpretação do modelo 1

Apresente os parâmetros do modelo obtido. Tentre mostrar as regras que são utilizadas no
processo de 'raciocínio' (*reasoning*) do sistema inteligente. Utilize medidas como 
o *feature importances* para tentar entender quais atributos o modelo se baseia no
processo de tomada de decisão.


### Resultados obtidos com o modelo 2.

Repita o passo anterior com os resultados do modelo 2.

### Interpretação do modelo 2

Repita o passo anterior com os parâmetros do modelo 2.


## Análise comparativa dos modelos

Discuta sobre as forças e fragilidades de cada modelo. Exemplifique casos em que um
modelo se sairia melhor que o outro. Nesta seção é possível utilizar a sua imaginação
e extrapolar um pouco o que os dados sugerem.


### Distribuição do modelo (opcional)

Tende criar um pacote de distribuição para o modelo construído, para ser aplicado 
em um sistema inteligente.


## 8. Conclusão

Apresente aqui a conclusão do seu trabalho. Discussão dos resultados obtidos no trabalho, 
onde se verifica as observações pessoais de cada aluno.

Uma conclusão deve ter 3 partes:

   * Breve resumo do que foi desenvolvido
	 * Apresenação geral dos resultados obtidos com discussão das vantagens e desvantagens do sistema inteligente
	 * Limitações e possibilidades de melhoria


# REFERÊNCIAS

Como um projeto de sistema inteligente não requer revisão bibliográfica, 
a inclusão das referências não é obrigatória. No entanto, caso você 
tenha utilizado referências na introdução ou deseje 
incluir referências relacionadas às tecnologias, padrões, ou metodologias 
que serão usadas no seu trabalho, relacione-as de acordo com a ABNT.

Verifique no link abaixo como devem ser as referências no padrão ABNT:

http://www.pucminas.br/imagedb/documento/DOC\_DSC\_NOME\_ARQUI20160217102425.pdf

Por exemplo:

**[1]** - _ELMASRI, Ramez; NAVATHE, Sham. **Sistemas de banco de dados**. 7. ed. São Paulo: Pearson, c2019. E-book. ISBN 9788543025001._

**[2]** - _COPPIN, Ben. **Inteligência artificial**. Rio de Janeiro, RJ: LTC, c2010. E-book. ISBN 978-85-216-2936-8._

**[3]** - _CORMEN, Thomas H. et al. **Algoritmos: teoria e prática**. Rio de Janeiro, RJ: Elsevier, Campus, c2012. xvi, 926 p. ISBN 9788535236996._

**[4]** - _SUTHERLAND, Jeffrey Victor. **Scrum: a arte de fazer o dobro do trabalho na metade do tempo**. 2. ed. rev. São Paulo, SP: Leya, 2016. 236, [4] p. ISBN 9788544104514._

**[5]** - _RUSSELL, Stuart J.; NORVIG, Peter. **Inteligência artificial**. Rio de Janeiro: Elsevier, c2013. xxi, 988 p. ISBN 9788535237016._



# APÊNDICES

**Colocar link:**

Do código (armazenado no repositório);

Dos artefatos (armazenado do repositório);

Da apresentação final (armazenado no repositório);

Do vídeo de apresentação (armazenado no repositório).




