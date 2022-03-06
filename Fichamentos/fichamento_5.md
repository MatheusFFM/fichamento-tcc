# Multi-discussing Across Issues in GitHub: A Preliminary Study

D. Hu, T. Wang, J. Chang, G. Yin and Y. Zhang, "Multi-Discussing across Issues in GitHub: A Preliminary Study," 2018 25th Asia-Pacific Software Engineering Conference (APSEC), 2018, pp. 406-415, doi: 10.1109/APSEC.2018.00055.

## 1. Fichamento de Conteúdo

O artigo busca investigar como desenvolvedores realizam multitarefas em nível de projeto e de _issues_. Diferentes estratégias e focos de _multi-discussing_ podem trazer diferentes influências no processo de resolução de _issues_, logo, o trabalho buscar responder se a _multi-discussing_ é uma prática comum na comunidade de desenvolvedores e como ela afeta na resolução de _issues_. Neste trabalho, foram coletados dados de diversos projetos _open source_ do GitHub, selecionando apenas projetos com mais de 3000 _issues_, totalizando 631 projetos para análise e coletando dados de _forks_, _issues_, estrelas e membros. Foi desenvolvido a partir desses dados uma métrica para representar o foco de discussão e então, foi realizado um modelo de regressão que encontrou uma média de 65% de _issues_ no conjunto de dados que possuem desenvolvedores aplicando a _multi-discussing_. O artigo também descobriu que a _multi-discussing_ normalmente traz benefícios para a resolução de uma _issue_ diminuindo sua latência, porém ela possui uma limitação em _issues_ com resoluções únicas. Com isso, percebe-se que essa prática é comum na comunidade e que ao alternar de _issues_, desenvolvedores conseguem receber mais oportunidades de aprendizado, otimizando seu tempo e esforço na maioria dos cenários.

## 2. Fichamento Bibliográfico 

* _multi-discussing_ (multidiscussão) é o fenômeno no qual desenvolvedores contribuem com comentários em diversas _issues_ e trocam a discussão entre elas (página 1).
* _DFocus_ é uma métrica elaborada para definir a taxa e a amplitude do foco dos desenvolvedores na troca de discussão em uma determinada semana (página 4).
* _avgFocus_ é uma métrica elabora para demonstrar a média do valor _DFocus_ de todos os desenvolvedores que discutiram em uma mesma _issue_ sem considerar o total de membros do projeto (página 5).

## 3. Fichamento de Citações 

* _"Multi-discussing can be seen as a kind of multitasking on the issue-level. "_
* _"We collect data from the population of open-source projects in GitHub. In this work, we obtain the data from GHTorrent. It is an effort to create a scalable, offline mirror of data offered through the Github REST API."_
* _"For the overall issue resolution, more multi-discussing tend to bring shorter average issue resolution latency."_
* _"We have found that the phenomenon of developers multidiscussing in multiple issues is common in GitHub projects."_
* _"In a single issue, more discussion-switching means less focus of developers, which may bring longer issue resolution latency."_
