# Conceitos Apresentados na Aula:

<br>

## O que é Processamento de Linguagem Natural (PLN) e suas aplicações no mundo real:

- Processamento de Linguagem Natural (PLN) é uma subárea da ciência da computação que tem como objetivo a interpretação e geração automática da linguagem natural humana. Integrando-se a áreas como inteligência artificial, aprendizado de máquina e linguística, o PLN trata da comunicação entre humanos e computadores por meio de textos ou fala. Esse campo lida com desafios como a compreensão e a geração de linguagem natural, buscando fazer com que computadores realizem tarefas úteis envolvendo a linguagem, como comunicação, tradução automática, análise de sentimentos e assistentes virtuais.

- O principal objetivo do PLN é automatizar a interpretação e geração da linguagem natural, ou seja, o idioma humano, seja ele falado ou em sinais. O processamento segue um fluxo de análise que começa com um corpus (conjunto de textos) e passa por pré-processamento, segmentação e outras análises para que a máquina possa entender o significado intencional. 

- A linguagem natural se refere a qualquer linguagem desenvolvida de forma espontânea pelos humanos, sem planejamento. Ao longo da história, acredita-se que ela surgiu há cerca de 50 mil anos na África, sendo essencial para a comunicação entre indivíduos, incluindo povos ancestrais. Embora se saiba pouco sobre como o cérebro humano processa a linguagem, alguns estudos sugerem uma relação entre o crescimento do cérebro humano e o surgimento da linguagem. 

- A fala, uma característica essencial da linguagem, é composta por palavras e seus elementos menores, como letras e sons, e pode variar no tempo e no espaço. Outro tipo de linguagem é a de sinais, que possui complexidades próprias e é também uma forma de comunicação humana. 

- O estudo do PLN é motivado pela necessidade de gerar e compreender automaticamente línguas humanas, permitindo que computadores realizem tarefas úteis que envolvem a linguagem, como a comunicação entre humanos e máquinas. O principal desafio do PLN é fazer com que os computadores entendam e gerem linguagem natural de forma eficaz para resolver problemas práticos. 

<br>

## Reconhecer os principais desafios envolvidos no processamento de linguagem humana:

O Processamento de Linguagem Natural (PLN) busca simular a compreensão da linguagem humana por máquinas, mas enfrenta uma série de desafios complexos. Esses desafios se assemelham às dificuldades que os humanos têm em interpretar a comunicação, embora as máquinas ainda careçam da capacidade cognitiva que nós desenvolvemos naturalmente. Alguns dos principais desafios no PLN incluem: 

- <b> Segmentação de Texto: </b> Separar frases e palavras em unidades significativas pode ser trivial em alguns casos, mas quando lidamos com dados complexos como gráficos ou abreviações, a segmentação torna-se difícil. Isso porque a máquina precisa identificar os limites entre frases ou elementos que nem sempre seguem padrões simples, como no caso de tabelas ou textos com formatação incomum. 

- <b> Análise de Contexto: </b> Compreender o contexto é essencial para interpretar corretamente a linguagem. Frases que compartilham palavras, mas possuem significados distintos em contextos diferentes, como no exemplo das palavras “colher” e “comer”, podem facilmente confundir a máquina. Métodos como gráficos de conhecimento ajudam na interpretação, mas ainda são limitados. 

- <b> Extração do Significado Semântico: </b> A compreensão da semântica vai além da simples identificação de palavras. Mesmo frases com vocabulário semelhante podem ter significados drasticamente diferentes, dependendo da ordem e do contexto das palavras. Para que a máquina tenha sucesso, ela precisa identificar essas nuances e não apenas palavras individuais. 

- <b> Ambiguidade: </b> Muitas palavras possuem múltiplos significados (ambiguidade semântica), o que torna o entendimento mais difícil para máquinas. Expressões ambíguas, como no exemplo da "cadeira" e "braço", requerem uma análise profunda para que o sentido correto seja identificado. 

- <b> Neologismos e Figuras de Linguagem: </b> Novos termos ou expressões populares, como gírias ou ironias, também são obstáculos, pois exigem uma flexibilidade que as máquinas ainda estão longe de alcançar. Além disso, o uso de abreviações e acrônimos na internet dificulta ainda mais o entendimento, pois a máquina precisa inferir o significado correto a partir de um contexto limitado. 

- <b> Resolução de Correferências: </b> Identificar corretamente quais palavras referem-se a quais entidades em um texto, como no exemplo "ele" e "Zezinho", é outra tarefa complexa. A capacidade de resolver correferências é crucial para a interpretação precisa de textos. 

<br>

## Conhecimentos de linguagens dos sistemas.

Os conhecimentos de linguagens dos sistemas são:

- Conhecimentos de fonéticas e fonologia 

- Reconhecimento de voz: sinal de voz >>> palavras 

- Sintetização de voz: palavras >>> sinal de voz



<br>

## Área de estudo da PLN.


- <b> Classificação de Textos: </b> Consiste em atribuir rótulos ou categorias predefinidas a textos. 

- <b> Detecção de Spam: </b> Identificação automática de e-mails indesejados (spam) ou não solicitados. 

- <b> Categorização de Texto: </b> Organizar textos em tópicos ou classes com base em seu conteúdo. 

- <b> Detecção de Intenção de Fala: </b> Identificar a intenção por trás de uma frase ou comando falado por um usuário. 

- <b> Extração de Informação: </b> Identificar e extrair automaticamente dados relevantes de textos. 

- <b> Recuperação de Informação: </b> Buscar e recuperar informações relevantes em grandes volumes de dados, como em motores de busca. 

- <b> Máquina de Tradução: </b> Traduzir automaticamente texto de uma língua para outra. 

- <b> Sumarização: </b> Gerar automaticamente uma versão condensada de um texto, mantendo as informações mais relevantes. 

- <b> Geração de Linguagem Natural: </b> Gerar texto ou frases de forma automática, geralmente para produzir respostas ou descrições em linguagem natural.




<br>

## Tarefas da PLN

Algumas das tarefas da PLN são:

- Todas as aplicações são construídas de forma modular a partir de uma ou mais tarefas computacionais sequenciais 

- Cada aplicação é construída de forma modular, e cada módulo realiza uma tarefa computacional específica que, por sua vez, produz uma saída. Essa saída se torna a entrada do próximo módulo, criando uma cadeia de processamento.  

- Como todo modelo computacional, cada tarefa computacional recebe uma entrada e retorna uma saída 

- Numa aplicação de PLN, a saída de um módulo é a entrada do módulo subsequente 