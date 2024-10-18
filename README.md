# EBA- Aula 09-Reressão Logística


Chegou a hora de treinarmos os conceitos sobre Regressão Logística das aulas anteriores. Este repositório é relativo a parte prática da aula 09, onde usamos a regressão logistica para classificar se um certo registro de um nódulo, tem ou não chance de ser benigno.


Chegou a hora de treinarmos os conceitos ensinados em aula!

Na pasta `data` você vai encontrar os dados em arquivo `csv`e `xlsx`. Na pasta `notebooks` você vai ter o gabarito proposto para a solução do exercício. Recomendamos que você tente fazer sozinho antes de olhar o gabarito. Isto vai fazer com que suas habilidades analíticas sejam desenvolvidas muito mais rapidamente.

## INSTRUÇÕES PARA RESOLUÇÃO DO CASE:


O conjunto de dados é composto por clientes da empresa Ifood com dados sobre:

- Perfis de clientes
- Preferências do produto
- Sucessos/fracassos da campanha
- Desempenho do canal

O **objetivo** de hoje é fazer uma análise exploratória desses dados. 

**Responda usando a sua ferramenta de preferência:**


1- Quantos dados temos? Linhas e colunas

2- Quais são as colunas numéricas?

3- Temos duplicados na nossa base? Se tivermos, retire-os.

3- Temos dados nulos nessa base? Será que eles indicam algo? O que fazer com eles?

4- Qual é a média, mediana, 25 percentil, 75 percentil, mínimo e máximo de cada uma das colunas numéricas? 

**Vamos agora entender o perfil de clientes que temos:**

1- Qual é o maior salário encontrado na nossa base? Veja na coluna `Income`!

2- Qual é a distribuição de salário na nossa base?

3-Temos clientes que ganham muito bem e outros que não ganham muito bem? Veja na coluna `Income`

4- Nossos clientes tem níveis de educação maiores ou menores? Veja na coluna `education_level`.

5- Quantos clientes temos em cada estado civil? Veja na coluna `marital_status`

**Agora vamos ver como os dados se correlacionam:**

1- Qual é a relação de estado civil com número de filhos? Será que as pessoas casadas têm um maior número de filhos? Filhos está na `coluna kids`

2- As pessoas gastam mais ou menos em nossa plataforma quando têm filhos? Veja nas colunas `expenses` e `kids`

3- Pessoas que têm um maior salário gastam mais? Veja nas colunas `Income` e `expenses`

#### Vá além! 

O que você faria com as informações que tirou das perguntas acima?
Trace um problema de negócios e faça quantas perguntas forem necessárias para respondê-la. 

Não esqueça de ir ao plantão de dúvidas e postar no discord caso haja dúvidas!


## INSTRUÇÕES PARA O USO DESTE REPOSITÓRIO:

### **Como utilizar este repositório?**

Este repositório contém os arquivos e códigos necessários para a aula de Estatística Descritiva. Abaixo estão as instruções simplificadas para configurar o ambiente com Pyenv e Poetry.

- **Passo a Passo para Configuração do Ambiente:**

1. **Clonar o Repositório:**

No terminal, clone este repositório:

```bash
git clone https://github.com/EbaPed/EBA-aula09-RegLogistica.git
cd EBA-aula09-RegLogistica
```

2. **Configurar a versão do Python com Pyenv**

Defina a versão do Python para o projeto. Para esta aula, vamos usar o Python 3.10.11 (ou outra versão compatível):

```bash
pyenv local 3.10.11
```

3. **Ativar o Ambiente Virtual Poetry**

Agora, ative o ambiente virtual:

```bash
poetry shell
```

4. **Instale as dependências do projeto usando Poetry:**

```bash
poetry install
```

Isso criará automaticamente um ambiente virtual isolado.


5. **Configurar o Kernel do Jupyter Notebook**

Se você for usar Jupyter Notebook, instale o ipykernel:

```bash
poetry add ipykernel
python -m ipykernel install --user --name=venv --display-name "Python (venv)
```

No Jupyter Notebook, escolha o kernel "Python (venv)" ao iniciar ou criar um novo notebook.


6. **Desativar o Ambiente Virtual**

Para sair do ambiente virtual, basta usar:

```bash
exit
```

7. **Executar o Código**

Agora que o ambiente está configurado, você pode executar os códigos Python fornecidos no repositório.

### **Comandos úteis**

- Ativar o ambiente virtual Poetry:

```bash
poetry shell
```

- Rodar um script com Poetry:

```bash
poetry run python script.py
```

- Adicionar bibliotecas:

 ```bash
poetry add nome_da_biblioteca
```

- Remover Bibliotecas:

 ```bash
poetry remove nome_da_biblioteca
```

