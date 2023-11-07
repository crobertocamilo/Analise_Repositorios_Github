## **Análise de dados dos repositórios mais populares do Github utilizando API**

Neste repositório, é feita a extração de dados a partir da [API do Github](https://api.github.com/search/repositories). Foram analisados os mil repositórios mais populares em número de estrelas (*Stars*) e em número de *Forks*.

O processo de extração e obtenção das bases de dados, bem como toda a análise é apresentanda no [**notebook**](https://github.com/crobertocamilo/Analise_Repositorios_Github/blob/main/analise.ipynb) Python neste repositório.

##

### Descrição da base dados:

Os arquivos [stars1000.csv](https://github.com/crobertocamilo/Analise_Repositorios_Github/blob/main/stars1000.csv) e [forks1000.csv](https://github.com/crobertocamilo/Analise_Repositorios_Github/blob/main/forks1000.csv), respectivamente, contém dados sobre os mil repositórios mais populares (Top1000) do Github em número de *Stars* e de *Forks*, no dia **5/11/2023**.

<br />

```markdown
Owner: Pessoa, empresa ou fundação dona do repositório

Name: Nome do repositório

URL: Endereço do repositório, identificador único composto pelo nome do responsável e nome do repositório

Stars: Número de vezes em que o repositório foi favoritado (marcado com estrela) à data da extração dos dados

Forks: Número de vez em que repositório foi copiado por outros usuários para sua área pessoal (feito um *Fork*) à data da extração dos dados

Branch Count: Número de *branches* no repositório

Created Date: Data de criação do repositório (formato yyyy-MM-dd)

Languanges: Lista de linguagens de programação utilizadas nos arquivos do repositório

Languages Proportion: Dicionário contendo o nome da linguagens e sua proporção (porcentagem de linhas de código) no projeto
```

##

### Resultados das Análises

As análise realizadas (implentação em código e discussão dos resultados) são apresentadas no [**notebook**](https://github.com/crobertocamilo/Analise_Repositorios_Github/blob/main/analise.ipynb) Python neste repositório.

<br />
<div align="center">
  <img src="https://github.com/crobertocamilo/Analise_Repositorios_Github/blob/main/assets/uso_linguagens_vs_idade_repositorio.png" alt="Exemplo de análise" width=100%/>
</div>

<div align="center">
Exemplo de análise - Participação das principais linguagens de progamação nos repositórios mais populares, em função do ano de criação (idade) do repositório.
</div>

##

### Conclusões

Neste trabalho, foi realizada a análise de dados dos repositórios mais populares do Github (em 05/11/2023) em número de estrelas (*Stars*) e de cópias (*Forks*). Estas métricas refletem o interesse da comunidade pelos projetos pois formas de obter acesso rápido à ele, favoritando-o (marcando com estrela), ou fazendo uma cópia dele para sua área pessoal (um *Fork*) para guardar ou para criar a partir dela.

Observou-se que as duas métricas estão associadas, com uma correlação de ~0.7, e que ambas tendem a serem maiores para repositórios mais antigos (dentre os Top1000). Uma quebra nesta tendência inclusive mostrou o enorme interesse despertado por repositórios relacioandos à *prompts* para ChatGPT e outras ferramentas de IA generativa.

Analisando a presença de proporção de linhas de código de cada linguagem, observou-se que linguagens de script e marcação como Shell, Dockerfile e o próprio HTML estão presente em grande parte dos projetos, mas são as linguagens de programação que apresentam uma maior participação nos repositórios. Calculando a proporção de uso das linguagens em função da idade dos repositórios, os resultados mostraram um crescimento na tendência de uso de Python e TypeScript, e de queda para JavaScript; C++, Java e Go oscilam ao longo dos anos, mas continuam entre as linguagens mais utilizada nos projetos. 

##
### Autor
[Carlos Roberto de Souza Camilo](https://www.linkedin.com/in/carlos-roberto-camilo/)  
Nov. 23