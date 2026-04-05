# Conjunto de dados sobre vício em redes sociais e produtividade

Um conjunto de dados realista que analisa o impacto do uso das redes sociais na produtividade.

## Visão geral

Este conjunto de dados explora a relação entre o uso de redes sociais e os níveis de produtividade entre indivíduos.

Ele reúne características comportamentais, hábitos de vida e padrões de atividade digital, simulando situações próximas do mundo real.

## Objetivo

O principal objetivo deste conjunto de dados é analisar como o uso de redes sociais pode estar associado à produtividade.

Com ele, é possível:

- investigar padrões de comportamento digital
- analisar fatores relacionados ao foco e à produtividade
- criar modelos de aprendizado de máquina para prever a pontuação de produtividade
- classificar os níveis de dependência em redes sociais

## Variáveis do conjunto de dados

- **age**: idade do indivíduo
- **daily_screen_time**: tempo total de uso de tela por dia, em horas
- **social_media_hours**: tempo gasto em redes sociais, em horas
- **study_hours**: tempo produtivo dedicado a estudo ou trabalho
- **sleep_hours**: duração diária do sono
- **notifications_per_day**: número de notificações recebidas por dia
- **focus_score**: pontuação de foco mental, variando de 0 a 100
- **addiction_level**: nível de dependência em redes sociais (`Low`, `Medium`, `High`)
- **productivity_score**: pontuação de produtividade, variando de 0 a 100

## Características dos dados

- 6000 linhas
- presença de valores ausentes em aproximadamente 2% dos dados
- correlações realistas entre variáveis
- adequado para tarefas de análise exploratória, regressão e classificação

## Possíveis aplicações

Este conjunto de dados pode ser utilizado para:

- realizar análise exploratória de dados (EDA)
- estudar o comportamento de dependência digital
- prever produtividade com modelos de aprendizado de máquina
- desenvolver técnicas de tratamento de dados e engenharia de atributos

## Como obter o conjunto de dados

O conjunto de dados está disponível no Kaggle: [Link para o dataset no Kaggle](https://www.kaggle.com/datasets/joaobrr/social-media-addiction-and-productivity-dataset) (substitua pelo link real se disponível).

Para baixar diretamente, use o comando Kaggle API:

```bash
kaggle datasets download -d joaobrr/social-media-addiction-and-productivity-dataset
```

## Instalação

Para trabalhar com este conjunto de dados, você precisará das seguintes bibliotecas Python:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Instale as dependências com:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Exemplo de uso

Aqui está um exemplo simples de como carregar e visualizar o conjunto de dados:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Carregar o conjunto de dados
df = pd.read_csv('social_media_addiction_dataset.csv')

# Visualizar as primeiras linhas
print(df.head())

# Gráfico de dispersão entre horas em redes sociais e produtividade
plt.scatter(df['social_media_hours'], df['productivity_score'])
plt.xlabel('Horas em Redes Sociais')
plt.ylabel('Pontuação de Produtividade')
plt.title('Relação entre Uso de Redes Sociais e Produtividade')
plt.show()
```

## Contribuição

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do repositório
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
