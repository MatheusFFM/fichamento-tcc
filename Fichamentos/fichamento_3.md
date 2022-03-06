# Anomalicious: Automated Detection of Anomalous and Potentially Malicious Commits on GitHub

D. Gonzalez, T. Zimmermann, P. Godefroid and M. Schaefer, "Anomalicious: Automated Detection of Anomalous and Potentially Malicious Commits on GitHub," 2021 IEEE/ACM 43rd International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP), 2021, pp. 258-267, doi: 10.1109/ICSE-SEIP52600.2021.00035.

## 1. Fichamento de Conteúdo

O artigo busca mostrar que _commits_ maliciosos podem ser detectados com alta acurácia a partir de um detector de anomalias focado na segurança da aplicação, essa ferramenta de detecção foi nomeada _Anomalicious_. A segurança é um dos fatores mais críticos em projetos _open source_, porém, pouco é discutido sobre soluções automáticas que buscam detectar e prevenir a infecção do repositório a partir de contribuições e dependências. O artigo notavelmente fomenta a tese de que o uso de componentes com vulnerabilidades conhecidas é um dos 10 maiores riscos de segurança de acordo com a _Open Web Application Security Project_ (OWASP), dando ainda mais importância para o trabalho. Dado isso, o trabalho gerou a ferramenta _Anomalicious_ que realiza a mineração de dados de _commits_ e metadados do repositório para entender o histórico do projeto e detectar possíveis anomalias em _commits_. A ferramenta busca atender cinco critérios: agnóstico de linguagem; ser personalizável; produzir alertas explicáveis; produzir alertas com baixa taxa positiva e detectar _commits_ maliciosos. Essa ferramenta faz a análise de fatores de histórico de arquivos, propriedades de alterações de _outliers_, _pull requests_, arquivos sensíveis e confiança do contribuidor, cada um desses tópicos analisa diferentes propriedades. Em um experimento realizado, foram coletados 100 repositórios repositórios de _Node Package Manager_ (NPM) com pelo menos 100 _commits_, nesse cenário a ferramenta apontou um baixo índice de resultados positivos, totalizando em 34 _commits_ apontados como suspeitos. Em outro experimento realizado no qual foram avaliados um conjunto de 15 cenários de _commits_ maliciosos, 8 deles foram detectados pela ferramenta, demonstrando que o modelo de regras da ferramenta pode ser refinado e treinado com uma base maior de dados de treinamento.


## 2. Fichamento Bibliográfico 

* _Factors_ (fatores) são propriedades de _commits_ ou contribuidores que podem indicar comportamento suspeito ou incomum, um conjunto de fatores desrespeitados podem indicar algo malicioso (página 1).
* _Sensitive files_ (arquivos sensíveis) são todos arquivos de extensões .xml, .json, .jar, .ini, .dat, .cnf, .yml, .toml, .gradle, .bin, .config, .exe, .properties, .cmd, .build (página 2).
* _Trust factors_ (fatores de confiança) é um valor computado a partir das seguintes propriedades de um contribuidor: nome de usuário identificável, idade da conta, número de commits, tempo desde o primeiro commit, distribuição de tempo de commit e proporção de pull requests rejeitados (página 3).
* _Data pipeline_ é o processo no qual os dados do repositório e dos _commits_ necessários para calcular cada fator são coletados, organizados e armazenados (página 2).

## 3. Fichamento de Citações 

* _"The main contribution (Section VI-A) of this work is showing that malicious commits can be detected with high accuracy using a security-focused rule-based anomaly detector relying only on commit-related metadata."_
* _"OSS projects face an increased risk of being compromised by malicious contributions"_
* _"After Anomalicious completes its analysis it produces a Commit Report detailing all violated rules and helpful contextual information for each flagged commit. "_
* _"When a commit is flagged, it is important for the reason to be explainable so that a repository maintainer can easily understand why the commit was flagged and quickly decide whether it is worth taking further action"_
