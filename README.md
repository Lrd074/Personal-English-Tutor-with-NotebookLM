# Professor Pessoal de Inglês com NotebookLM

## 1. Contexto e objetivo

Este projeto surgiu a partir do interesse em utilizar Inteligência Artificial não apenas como ferramenta para responder dúvidas, mas como uma ferramenta de apoio contínuo ao processo de aprendizagem.

O objetivo foi construir, utilizando o **NotebookLM**, um ambiente de estudo capaz de funcionar como um **professor pessoal de inglês**, orientando as aulas a partir de fontes previamente selecionadas sobre metodologias de ensino, aprendizagem de idiomas, conteúdos de inglês e materiais didáticos.

A proposta não foi simplesmente fornecer ao NotebookLM conteúdos sobre inglês. A ideia foi criar uma estrutura em que diferentes fontes pudessem sustentar a forma como o ensino seria conduzido.

O projeto foi organizado em quatro pilares:

* Metodologias gerais de ensino;
* Metodologias específicas para o ensino de inglês;
* Conteúdos e assuntos que devem ser estudados durante a aprendizagem;
* Materiais didáticos e conteúdos voltados ao nível iniciante.

O objetivo final é fazer com que a IA não funcione apenas como um gerador de exercícios, mas como um **ambiente de aprendizagem adaptativo**, capaz de identificar dificuldades, propor atividades contextualizadas, corrigir erros, acompanhar a evolução e determinar quando existe evidência suficiente para avançar.

### Objetivos de estudo

Os principais objetivos do projeto são:

1. Desenvolver uma metodologia personalizada para aprendizagem de inglês.
2. Utilizar IA como ferramenta de acompanhamento contínuo dos estudos.
3. Transformar conhecimento passivo em conhecimento ativo por meio de prática e produção.
4. Desenvolver progressivamente compreensão, vocabulário, gramática em uso, leitura, escrita, compreensão auditiva e comunicação.
5. Evitar a progressão baseada apenas na conclusão de conteúdos ou no acerto isolado de exercícios.
6. Criar um sistema que identifique lacunas e proponha revisões antes da progressão.
7. Testar diferentes formas de engenharia de prompts para melhorar a qualidade das aulas geradas pela IA.

---

# 2. Estrutura do NotebookLM

Inicialmente, o NotebookLM foi configurado com a orientação de funcionar como um **guia de aprendizado**.

A intenção foi estabelecer primeiro a função que a IA deveria desempenhar antes de definir detalhadamente como cada aula seria conduzida.

A estrutura utilizada considera que aprender inglês não significa apenas memorizar regras gramaticais. O estudante precisa conseguir reconhecer estruturas, compreender seu funcionamento e, principalmente, utilizá-las em situações reais.

Por isso, o notebook foi orientado a trabalhar com:

**Reconhecimento → Compreensão → Prática → Produção → Avaliação → Revisão → Progressão**

Esse ciclo procura evitar um problema comum em processos de aprendizagem mediados por IA: o estudante conseguir responder corretamente a exercícios, mas não conseguir utilizar o conhecimento espontaneamente.

---

# 3. Curadoria das fontes

As fontes foram selecionadas com diferentes funções dentro do projeto. Em vez de utilizar somente materiais diretamente relacionados ao inglês, foram combinados conteúdos sobre educação, metodologias de ensino, aprendizagem de idiomas e materiais didáticos.

## 3.1 Metodologias gerais de ensino

### Vídeo — Metodologias de ensino

https://www.youtube.com/watch?v=4XnBpAvQF6Q

Utilizado como referência para compreender princípios e abordagens gerais relacionados ao processo de ensino e aprendizagem.

### TutorMundi — Métodos de ensino

https://tutormundi.com/blog/metodos-de-ensino/

Fonte utilizada para complementar o estudo das diferentes metodologias e estratégias de ensino.

---

## 3.2 Metodologias específicas para o ensino de inglês

### Vídeo — Metodologias para aprendizagem de inglês

https://www.youtube.com/watch?v=_oZ1eZqQT98

Utilizado como referência para metodologias aplicadas especificamente ao ensino e aprendizagem da língua inglesa.

### TopWay — Metodologia imersiva para aprender inglês

https://www.topwayschool.com/blog/metodologia-imersiva-aprender-ingles

Fonte utilizada para compreender o conceito de imersão e sua aplicação no aprendizado de idiomas.

---

## 3.3 Conteúdos e assuntos para estudar inglês

### Curso/playlist de inglês

https://www.youtube.com/watch?v=X5TdMsc4YCg&list=PL41dMNqXopt85RhRgFp_jdoI5Bz7DUG-c

Utilizado como referência para identificar conteúdos e assuntos que podem compor uma progressão de estudos.

### TopWay — Lista de assuntos para estudar inglês

https://www.topwayschool.com/blog/lista-assuntos-estudar-ingles

Utilizado como referência complementar para organização dos conteúdos de aprendizagem.

---

## 3.4 Material didático

### Apostila de Inglês para Iniciantes

https://www.kufunda.net/publicdocs/cliqueapostilas-apostila-de-ingles-para-iniciantes.pdf

Utilizada como material de apoio para conteúdos e exercícios relacionados ao nível iniciante.

---

# 4. Engenharia de Prompts

A engenharia de prompts foi utilizada para definir não somente **o que a IA deveria ensinar**, mas principalmente **como ela deveria ensinar**.

Foram utilizados dois prompts principais.

## 4.1 Prompt inicial

O primeiro prompt teve uma função mais simples:

> "Aprender inglês."

A partir dele, os demais pilares do notebook passaram a funcionar como suporte para as aulas de inglês, utilizando as fontes sobre metodologias, métodos, técnicas de estudo e conteúdos.

Essa primeira abordagem serviu como ponto de partida, mas apresentava uma limitação importante: uma instrução muito genérica não define suficientemente o comportamento esperado do professor.

Isso levou à elaboração de um segundo prompt, muito mais específico.

---

# 5. Prompt principal

O segundo prompt foi desenvolvido para transformar a IA em um professor mais estruturado e adaptativo.

```text
Meu nível é iniciante.

NÃO avance automaticamente de etapa. Ao concluir cada estágio, aplique um teste de progressão. Avalie, conforme o nível, compreensão, vocabulário, gramática em uso, leitura, escrita, compreensão auditiva e produção. Priorize tarefas práticas e contextualizadas. Analise meus erros, identifique lacunas e determine se estou apto a avançar. Se não estiver, revise os pontos necessários e reavalie. Só avance com evidência suficiente de domínio.

Meu perfil: aprendo melhor de forma prática, contextualizada e progressiva. Gosto de entender o motivo por trás das coisas; não quero apenas decorar regras. Preciso compreender como e por que uma estrutura é utilizada. Aprendo melhor com situações reais e prática imediata. Prefiro exemplos, diálogos, textos e exercícios contextualizados a aulas teóricas ou baseadas em memorização.

Apresente primeiro o desafio e aguarde minha tentativa. Depois, corrija e explique meus erros sem interromper excessivamente meu raciocínio. Diferencie erros relevantes de pequenos detalhes.

Tenho tendência a me aprofundar demais em assuntos específicos. Equilibre profundidade e progresso: responda dúvidas relevantes, mas não deixe que uma questão desvie toda a aula. Se não for essencial, registre-a para depois.

Estruture o ensino baseado nas metodologias salvas nas fontes, sempre se adaptando ao meu estilo de aprendizado.

Não quero apenas acertar exercícios de gramática: quero compreender textos e conversas, formular frases naturalmente, comunicar ideias e progressivamente pensar e me expressar em inglês. Considere que compreender uma explicação em português não significa conseguir utilizar uma estrutura em inglês. Transforme conhecimento passivo em conhecimento ativo por meio de produção e prática.

Use português nas explicações quando necessário, mas aumente progressivamente o inglês. Não traduza tudo automaticamente. Quando possível, faça-me inferir significados pelo contexto. Ensine vocabulário e gramática em situações reais.

Mantenha um registro do que aprendi, dificuldades recorrentes, erros frequentes, vocabulário estudado e habilidades que precisam de reforço. Ao final de cada aula, informe brevemente o que foi aprendido e pontos de atenção. Não presuma domínio por um acerto isolado: diferencie reconhecimento, compreensão e uso.
```

---

# 6. "Cicatrizes" e troubleshooting

Durante a construção do prompt, um dos principais problemas identificados foi que simplesmente informar à IA que o objetivo era **"aprender inglês"** não era suficiente para garantir uma metodologia consistente.

Uma instrução genérica poderia resultar em:

* aulas excessivamente teóricas;
* exercícios descontextualizados;
* avanço prematuro de conteúdo;
* excesso de tradução;
* foco excessivo em gramática;
* explicações antes da tentativa do aluno;
* confusão entre acertar uma questão e realmente dominar uma habilidade.

A solução encontrada foi transformar preferências e dificuldades de aprendizagem em **regras explícitas de comportamento para a IA**.

Por exemplo, em vez de simplesmente solicitar exercícios, o prompt determina:

> "Apresente primeiro o desafio e aguarde minha tentativa."

Isso altera a dinâmica da aula, fazendo com que a IA deixe de fornecer imediatamente a resposta.

Da mesma forma, a instrução:

> "Não presuma domínio por um acerto isolado: diferencie reconhecimento, compreensão e uso."

foi utilizada para tentar evitar uma avaliação superficial do progresso.

Outro ponto importante foi estabelecer um mecanismo de progressão:

> "Só avance com evidência suficiente de domínio."

Assim, a progressão passa a depender do desempenho demonstrado pelo estudante e não simplesmente da quantidade de conteúdos estudados.

---

# 7. Miniguia de estudo

## 7.1 Princípio central

O processo de aprendizagem proposto pelo projeto pode ser representado da seguinte maneira:

**Exposição → Compreensão → Prática → Produção → Feedback → Revisão → Avaliação → Progressão**

A exposição apresenta o conteúdo.

A compreensão busca entender o significado e o funcionamento da estrutura.

A prática permite utilizar o conhecimento em atividades controladas.

A produção exige que o estudante utilize o inglês para expressar suas próprias ideias.

O feedback identifica erros e lacunas.

A revisão trabalha os pontos que ainda não foram consolidados.

A avaliação verifica se o conhecimento está suficientemente desenvolvido.

Somente então ocorre a progressão.

---

# 8. Habilidades acompanhadas

O professor pessoal deve acompanhar diferentes dimensões da aprendizagem:

| Habilidade           | Objetivo                                               |
| -------------------- | ------------------------------------------------------ |
| Compreensão          | Entender o significado de palavras, frases e situações |
| Vocabulário          | Ampliar e utilizar palavras e expressões               |
| Gramática            | Compreender e utilizar estruturas corretamente         |
| Leitura              | Compreender textos progressivamente mais complexos     |
| Escrita              | Produzir frases e textos próprios                      |
| Compreensão auditiva | Entender inglês falado em diferentes contextos         |
| Produção             | Formular e comunicar ideias em inglês                  |

Um ponto fundamental do projeto é não tratar essas habilidades como equivalentes.

Um estudante pode reconhecer uma estrutura durante um exercício e ainda não conseguir utilizá-la espontaneamente em uma conversa.

Por isso, o projeto diferencia:

**Reconhecer ≠ Compreender ≠ Utilizar**

---

# 9. Glossário

**Input:** contato do estudante com a língua por meio de leitura, áudio, vídeos e outros materiais.

**Output:** produção realizada pelo estudante, como falar ou escrever em inglês.

**Contextualização:** apresentação de vocabulário e estruturas dentro de situações que possuem significado para o estudante.

**Imersão:** exposição significativa e progressiva ao idioma, reduzindo a dependência da tradução.

**Feedback:** retorno sobre o desempenho, incluindo identificação e explicação de erros.

**Progressão:** avanço para conteúdos ou habilidades mais complexos após evidências de aprendizagem suficiente.

**Conhecimento passivo:** aquilo que o estudante consegue reconhecer ou compreender, mas ainda não consegue utilizar com autonomia.

**Conhecimento ativo:** capacidade de utilizar determinado conhecimento para produzir linguagem.

**Aprendizagem adaptativa:** processo no qual o ensino é ajustado de acordo com o desempenho, dificuldades e características do estudante.

**Engenharia de prompts:** processo de elaboração e refinamento de instruções para orientar o comportamento e as respostas de um modelo de IA.

**Teste de progressão:** avaliação utilizada para verificar se o estudante apresenta evidências suficientes para avançar.

---

# 10. Prompts reutilizáveis

Além do prompt principal, a estrutura criada pode ser utilizada para gerar prompts específicos durante o processo de aprendizagem.

### Revisão

```text
Analise os conteúdos que já estudei e crie uma revisão baseada principalmente nos meus erros e dificuldades recorrentes.

Não apresente apenas exercícios de memorização. Misture reconhecimento, compreensão e produção.

Comece pelas dificuldades mais importantes e só aumente a dificuldade quando meu desempenho demonstrar domínio.
```

### Conversação

```text
Simule uma situação real de conversação em inglês adequada ao meu nível.

Não forneça minhas respostas. Apresente uma situação e aguarde minha tentativa.

Após minha resposta, corrija os erros mais relevantes, explique o motivo da correção e continue a conversa.

Priorize comunicação natural em vez de corrigir pequenos detalhes que não prejudicam a compreensão.
```

### Leitura

```text
Apresente um texto em inglês adequado ao meu nível.

Não traduza o texto imediatamente.

Faça perguntas de compreensão e permita que eu tente inferir o significado de palavras e expressões pelo contexto.

Depois da minha tentativa, explique os pontos que eu não compreendi e destaque vocabulário relevante.
```

### Diagnóstico

```text
Faça uma avaliação diagnóstica do meu inglês.

Avalie separadamente compreensão, vocabulário, gramática em uso, leitura, escrita e produção.

Não considere apenas respostas corretas. Analise meus erros, hesitações, padrões de dificuldade e capacidade de utilizar o conhecimento.

Ao final, indique quais habilidades precisam de maior atenção antes de avançarmos.
```

### Teste de progressão

```text
Aplique um teste para verificar se estou preparado para avançar para o próximo estágio.

Misture questões de compreensão, vocabulário, gramática em uso e produção.

Não revele as respostas antes da minha tentativa.

Depois de corrigir, determine se há evidências suficientes de domínio. Caso contrário, identifique exatamente quais pontos precisam ser revisados antes de uma nova tentativa.
```

---

# 11. Resultado esperado

O resultado final deste projeto não é simplesmente um chatbot que responde perguntas sobre inglês.

A proposta é construir um **ambiente de aprendizagem personalizado**, no qual a IA utilize fontes previamente selecionadas para orientar a metodologia e, ao mesmo tempo, adapte a prática ao desempenho do estudante.

O projeto também demonstra uma aplicação prática de Engenharia de Prompts: a qualidade do resultado não depende somente da pergunta "certa", mas da definição clara de contexto, objetivo, comportamento esperado, critérios de avaliação e mecanismos de correção.

A principal ideia aprendida durante o desenvolvimento foi que **uma IA pode produzir uma resposta correta sem necessariamente produzir um processo de aprendizagem eficiente**.

Por isso, o projeto buscou sair da lógica de:

**"Perguntar → Receber resposta"**

para uma lógica de:

**"Tentar → Receber feedback → Identificar lacunas → Praticar → Avaliar → Consolidar → Avançar"**

Essa mudança representa o principal objetivo do projeto: utilizar IA não apenas para fornecer conteúdo, mas para estruturar e acompanhar o processo de aprendizagem.
