# Lighthouse_DataScience
# Nome do Projeto
LH_CD_IAN_LUCAS_PERIGO_VIANNA

## Descrição
Projeto de ciência de dados e Machine learning para o processo seletivo para a vaga de trainee da LightHouse e Indicium.
Projeto feito entre o dia 15/02/2024 e 21/02/2024
Autor do projeto: Ian Lucas Périgo Vianna

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?style=flat-square&logo=linkedin&labelColor=blue)](https://www.linkedin.com/in/ianperigo)
[![E-mail](https://img.shields.io/badge/E--mail-Enviar%20E--mail-brightgreen?style=flat-square&logo=gmail&labelColor=brightgreen)](mailto:seu-ian.perigo.v@egmail.com)


## Pré-requisitos

- Python (versão X.X.X)
- Jupyter Notebook
- Outras dependências (se houver)

## Instalação

1. Clone o repositório:

    ```bash
    git clone [https://github.com/seu-usuario/seu-projeto.git](https://github.com/IanPerigoVianna/Lighthouse_DataScience.git)
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd seu-projeto
    ```

3. Instale as dependências:

    ```bash
    pip install -r requirements.txt
    ```

## Execução

1. Abra o notebook no Jupyter:

    ```bash
    jupyter notebook nome_do_notebook.ipynb
    ```

2. Execute as células conforme necessário.

## Carregando o Modelo Salvo

Se você deseja carregar um modelo treinado salvo com o `pickle`, siga estas etapas:

1. Abra um novo notebook ou utilize uma célula no mesmo notebook.

2. Importe a biblioteca `pickle`:

    ```python
    import pickle
    ```

3. Carregue o modelo e o objeto de preparação de dados:

    ```python
    # Carregue o modelo
    with open('model.pkl', 'rb') as model_file:
        loaded_model = pickle.load(model_file)

    # Carregue o objeto de preparação de dados (se aplicável)
    with open('scaler.pkl', 'rb') as scaler_file:
        loaded_scaler = pickle.load(scaler_file)
    ```

4. Utilize o modelo carregado para fazer previsões:

    ```python
   ###################### DOCUMENTAÇÃO DE INPUT DAS CHAVES PARA PREVISÃO DO PREÇO DO IMÓVEL #########################

 - Room_type preencha 1  em room_type entire home/apt caso o aluguel seja do imóvel completo e 0 caso não seja. ######################
 - Room_type preencha 1  em room_type shared caso o aluguel seja de quarto compartilhado 0 caso não seja.
 - Bairro_group preencha 1 para se o imóvel está localizado nesse bairro_group e 0 caso ele não esteja.
 - Bairro preencha 1 caso o imóvel esteja neste bairro e 0 caso não esteja
 - Disponibilidade 365_ preencha a quantidade de dias que o imóvel está disponível por ano
 - Calculado host_listening_counts preencha com a quantidade de anuncios do imóvel
 - Numero_de_reviews preencha com a quantidade de avaliações que o imóvel tem.

    prediction = loaded_model.predict(input_data_normalized)
    print(f"Previsão: {prediction}")

    Sugestão de preço original: $261.22
    ```

Lembre-se de substituir os nomes do arquivo (`model.pkl` e `scaler.pkl`) pelos reais que você usou ao salvar os objetos com o `pickle`.

