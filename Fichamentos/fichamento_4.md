# Pull Request Prioritization Algorithm based on Acceptance and Response Probability

M. I. Azeem, Q. Peng and Q. Wang, "Pull Request Prioritization Algorithm based on Acceptance and Response Probability," 2020 IEEE 20th International Conference on Software Quality, Reliability and Security (QRS), 2020, pp. 231-242, doi: 10.1109/QRS51102.2020.00041.

## 1. Fichamento de Conteúdo

O artigo busca propor uma abordagem chamada _Acceptance and Response based Prioritizer (AR-Prioritizer)_ que automaticamente classifica _pull requests_ de acordo com suas probabilidades de aceitação e resposta a fim de priorizar aqueles mais importantes. Com isso, o artigo aplica diversas técnicas de _machine learning_ a fim de avaliar a melhor performance de classificação. O desenvolvimento da abordagem, foram extraídos valores de recursos relacionados ao projeto, _pull requests_, autores e contribuidores, _integrators_ e _target labels_, em seguida é realizada a partir desses dados a predição da probabilidade do _pull request_ ser aceito e após isso, a probabilidade do _pull request_ receber uma atualização do usuário no dia atual, por fim, é desenvolvida uma função de valor que combina ambas as probabilidades. Os repositórios foram selecionados de acordo com a popularidade em estrelas e com uma média de 7 anos de história utilizando a GitHub REST API V3, resultando em 278,418 _pull requests_ de 19 projetos. Como resultado, a abordagem _AR-Prioritizer_ consegue recomendar os 5, 10 e 20 primeiros _pull requests_ a serem priorizados com uma média de precisão respectivamente de 95,3%, 89,6% e 79,6%, demonstrando possuir bons números em suas análises.

## 2. Fichamento Bibliográfico

* _Integrators_ (integradores) são valores que consideram a revisão de códigos do _pull request_, como número de comentários, discussões e participantes (página 3).
* _target labels_ (rótulos de destino) são variáveis dependentes utilizadas no conjunto de dados, como por exemplo, uma variável binária que representa se um _pull request_ foi ou não aceito (página 3).
* _XGBoost Model_ é um algoritmo de aprendizado de máquina baseado em árvore de decisão que usa uma estrutura de aumento de gradiente (página 2).

## 3. Fichamento de Citações

* _"[...] popular GitHub projects such as Kubernetes and Rails receive tens or hundreds of PRs daily. Selecting what PRs to accept or to what PRs to respond becomes a challenge for the integrators, even more so since the aforementioned platforms do not provide mechanisms for prioritizing PRs when they are submitted"_
* _"In particular, our prioritization approach is designed for giving the highest priority to PRs having both high acceptance and high response probabilities for supporting integrator(s) in providing feedback to contributors on PRs that are worthy to be accepted"_
* _"Our best performing models, i.e. XGB, have significantly outperformed the baseline models Gousios et al. and PRioritizer in acceptance and response prediction tasks respectively. Similarly, XGB models performed well in both the training strategies"_
* _"AR-Prioritizer has outperformed the baseline models in top@10 MAP and AR with a statistical significance. The prioritization is mainly driven by the response likelihood prediction while the acceptance dimension could serve to optimize the final rankings."_
