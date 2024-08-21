# Stock Agents

Este projeto foi desenvolvido durante o curso **IA na prática** da Rocketseat. O **Stock Agents** é um agente inteligente que utiliza a tecnologia LLM da OpenAI, especificamente o modelo `gpt-3.5-turbo`, para analisar o mercado de ações e fornecer previsões sobre o futuro das ações.

## Sobre o Projeto

O agente realiza a análise do histórico de preços de uma ação utilizando a API do **Yahoo Finance** e busca notícias relacionadas à empresa por meio do **DuckDuckGo**. Com base nas informações coletadas, ele tenta prever a tendência futura da ação — se vai subir, descer ou se manter estável — e oferece recomendações.

### Tecnologias Utilizadas

- **crewai**: Framework para desenvolvimento de agentes inteligentes.
- **yfinance**: Biblioteca para obtenção de dados financeiros históricos.
- **langchain**: Ferramenta para criação de cadeias de linguagem natural.
- **OpenAI GPT-3.5-turbo**: Modelo de linguagem natural utilizado para a análise e previsão.

### Importante

Este projeto foi desenvolvido com fins educacionais e **não substitui** a análise de um especialista financeiro. As previsões e recomendações feitas pelo agente devem ser utilizadas apenas como parte do processo de aprendizado.

## Como Usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/stock-agents.git
   ```

2. Instale as dependências:
  ```bash
  pip install -r requirements.txt
  ```  

3. Configure suas chaves de API. Certifique-se de definir a chave da OpenAI:

  ```python
  os.environ['OPENAI_API_KEY'] = st.secrets['OPENAI_API_KEY']
  ```

4. Execute o agente:
  ```bash
  python crewai-stocks.py
  ```

## Projeto Online

Você também pode ver o projeto em funcionamento no seguinte link:

[Stock Agents - Online](https://crewai-stockspy-9amjsvgtxrbflpseq5pm6w.streamlit.app/)