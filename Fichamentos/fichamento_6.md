# Using Dynamic and Contextual Features to Predict Issue Lifetime in GitHub Projects

R. Kikas, M. Dumas and D. Pfahl, "Using Dynamic and Contextual Features to Predict Issue Lifetime in GitHub Projects," 2016 IEEE/ACM 13th Working Conference on Mining Software Repositories (MSR), 2016, pp. 291-302.

## 1. Fichamento de Conteúdo

O artigo busca abordar o problema de prever, em um determinado ponto do tempo uma _issue_ será ou não finalizada, uma vez que métodos para prever o tempo de vida de _issues_ ajudam gerentes de projetos de software a priorizar as _issues_ e o alocamento de recursos. Estudos anteriores consideravam apenas aspectos estáticos da _issue_, enquanto este trabalho visa analisar propriedades do projeto como um todo. Esse projeto tenta buscar quais propriedades são importantes para definir o tempo de vida de uma _issue_ e a acurácia de uma análise estática e dinâmica de propriedades do contexto da _issue_. A seleção de repositórios do artigo abrange um período de 3 anos, totalizando 4024 projetos após uma filtragem de suas características, dentre eles, há um total de 967037 _issues_ coletadas, sendo 69.9% delas fechadas. Esse projeto aplica uma inteligência artificial supervisionada, algumas das características utilizadas foram o número de comentários, pontuação textual, número de atores e outras características relacionadas à própria _issue_, aos participantes, ao projeto e ao apresentador da _issue_. Como resultado, as propriedades que mais ajudaram na predição do tempo de vida foram o número de _issues_ criadas e fechadas dentro de um período antes da criação da _issue_ analisada. Além disso, a partir da análise da acurácia obtida, a conciliação entre as características dinâmicas e contextuais complementam o poder preditivo das análise estática especialmente para previsões de longo prazo.

## 2. Fichamento Bibliográfico 

* _Sticky issue_ (Problemas fixos) são _issues_ que não foram finalizadas dentro durante o período de observação do trabalho (página 3).
* _Random Forest_ (Floresta aleatória) é um classificador que treina várias árvores de decisões nos mesmos dados, mas em cada uma há um conjunto aleatório dos dados (página 6).
* _F1-score_ coloca em evidência casos de modelos abaixo da média, no caso, mesmo que eles identifiquem as _issues_ próximas do fechamento, eles possuem baixa precisão ou baixa revocação (página 6).

## 3. Fichamento de Citações 

* _"Having an estimate of issue closing time can help to reduce this uncertainty and provide greater transparency to all stakeholders"_
* _"an estimate of issue closing time provides core team members with a basis to prioritize their efforts and plan their contributions."_
* _"The predictive models studied in this paper benefit from being trained on a large dataset. The counter-part of this benefit is that the set of projects in the dataset are very heterogeneous, making the prediction problem more difficult."_
* _"The observed accuracy of our models (AUC and precision scores) suggests that predictive models of issue lifetime across large sets of open source projects could potentially be used in practice if users were willing to tolerate some fluctuation in their predictive accuracy"_
