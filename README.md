# python_power_up
Automação com Python
# 🖥️ Automação de Cadastro de Produtos

Este projeto tem como objetivo automatizar o processo de **login em um sistema web** e **cadastro de produtos** utilizando **Python** e a biblioteca [PyAutoGUI](https://pyautogui.readthedocs.io/).

---

## 🚀 Funcionalidades

- Abre o navegador automaticamente e acessa o sistema da empresa.  
- Realiza o login com credenciais pré-definidas.  
- Lê uma base de dados em **CSV** (`produtos.csv`) contendo os produtos a serem cadastrados.  
- Preenche automaticamente os formulários de cadastro no sistema web.  
- Cadastra todos os produtos de forma sequencial.  
- Permite capturar a posição do mouse na tela para ajustar os pontos de clique.  

---

## 📂 Estrutura do Projeto

```
📦 projeto-automacao
 ┣ 📜 codigo.py          # Script principal da automação
 ┣ 📜 pegar_posicao.py   # Script auxiliar para capturar coordenadas do mouse
 ┣ 📜 produtos.csv       # Base de dados com os produtos a cadastrar
 ┗ 📜 README.md          # Documentação do projeto
```

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- [PyAutoGUI](https://pyautogui.readthedocs.io/) → Automação de cliques, teclas e digitação  
- [Pandas](https://pandas.pydata.org/) → Leitura e manipulação do arquivo CSV  
- **CSV** → Base de dados de produtos  

---

## 📋 Pré-requisitos

Antes de executar, certifique-se de ter instalado:

```bash
pip install pyautogui pandas
```

---

## ▶️ Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Entre na pasta do projeto:
   ```bash
   cd projeto-automacao
   ```
3. Ajuste as posições do mouse:
   - Execute o script:
     ```bash
     python pegar_posicao.py
     ```
   - Posicione o mouse no campo desejado em até **5 segundos** → a posição será exibida no terminal.  
   - Substitua as coordenadas no `codigo.py`.  

4. Execute a automação:
   ```bash
   python codigo.py
   ```

---

## 📊 Estrutura do CSV (`produtos.csv`)

O arquivo **produtos.csv** deve conter as seguintes colunas:

| codigo | marca | tipo | categoria | preco_unitario | custo | obs |
|--------|-------|------|-----------|----------------|-------|-----|

Exemplo:

```csv
codigo,marca,tipo,categoria,preco_unitario,custo,obs
123,MarcaX,Eletrônico,Informática,1500,1000,"Produto em promoção"
456,MarcaY,Acessório,Telefonia,200,120,
```

---

## ⚠️ Observações Importantes

- Os **valores de coordenadas (x, y)** podem variar de acordo com a resolução da sua tela → use o `pegar_posicao.py` para calibrar.  
- O script está configurado para abrir o **Google Chrome**. Caso use outro navegador, altere no código.  
- Utilize este projeto apenas para **fins educacionais** ou em **sistemas de teste**, nunca em ambientes de produção sem autorização.  

---
