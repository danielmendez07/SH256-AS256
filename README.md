# Projeto: AES-256 e SHA-256

## Método Utilizado

Durante os testes, utilizamos duas técnicas fundamentais de segurança digital: a função de hash **SHA-256**, implementada pela biblioteca `hashlib`, e a criptografia simétrica **AES-256**, disponibilizada pela biblioteca `cryptography`. O propósito foi ilustrar as operações e as diferenças principais entre criptografia e hashing.

### SHA-256
Selecionamos cinco strings variadas, incluindo textos com caracteres especiais, para passar pela função de hash SHA-256. Isso demonstrou a capacidade dessa função de gerar um valor de hash único e de tamanho fixo para cada entrada diferente, ressaltando sua utilidade em produzir resumos consistentes de dados.

### AES-256
Escolhemos cinco strings para serem criptografadas utilizando uma chave e um vetor de inicialização (IV) aleatórios para cada teste. A reversibilidade foi testada por meio da descriptografia das mensagens criptografadas usando a mesma chave e IV, validando a eficácia e segurança da criptografia AES-256.

## Resultados Obtidos

Os testes com **SHA-256** confirmaram que a função de hash sempre produz um valor de tamanho fixo, independentemente do tamanho ou tipo dos dados de entrada. Esse comportamento sublinha a propriedade de produção de um resumo único para dados variados.

Nos testes de **AES-256**, observamos que a criptografia transforma a entrada em um conjunto de bytes que parece aleatório, mas que pode ser revertido para a forma original com o processo de descriptografia adequado. Isso demonstra a natureza reversível e segura do AES-256 para a proteção de dados.

## Comparação entre AES-256 e SHA-256

A diferença fundamental entre AES-256 e SHA-256 está na finalidade e na reversibilidade de seus processos:

- **SHA-256** é uma função de hash, designada para a verificação de integridade e autenticação de dados, produzindo uma "impressão digital" única dos dados que não pode ser revertida para formar original.

- **AES-256** é um algoritmo de criptografia, usado para a segurança na transmissão de informações, permitindo a criptografia e descriptografia dos dados com a utilização de uma chave secreta.

Enquanto o SHA-256 garante a integridade e autenticação, o AES-256 protege a confidencialidade dos dados, cada um desempenhando um papel vital na segurança da informação com aplicações específicas conforme as necessidades de segurança.


# Para testar o código em `main.ipynb`:

## Criação de Ambiente Virtual e Instalação de Dependências em Python

Para gerenciar as dependências de projetos Python de forma eficaz, é recomendável usar ambientes virtuais. 

### Passos para a Criação de um Ambiente Virtual e Instalação dos Requisitos

#### 1. Criação de um Ambiente Virtual

Para criar um novo ambiente virtual, navegue até o diretório do seu projeto e execute o seguinte comando:

```bash
python -m venv env
```

### 2. Ativação do Ambiente Virtual

Após a criação do ambiente virtual, você precisa ativá-lo:

- **No Windows:**
```bash
env\Scripts\activate
```

- **No macOS e Linux:**
```bash
source env/bin/activate
```

### 3. Instalação das Dependências

Com o ambiente virtual ativado, você pode instalar todos os pacotes necessários listados em `requirements.txt` usando pip:

```bash
pip install -r requirements.txt
```

### 4. Desativação do Ambiente Virtual

Quando terminar o trabalho no ambiente virtual, você pode desativá-lo com o seguinte comando:

```bash
deactivate
```

Isso retornará você ao ambiente global do Python no seu sistema.


## Execução do Código

Após a instalação das dependências e a ativação do ambiente virtual, você pode executar o código em `main.ipynb` em um ambiente Jupyter Notebook ou JupyterLab.










