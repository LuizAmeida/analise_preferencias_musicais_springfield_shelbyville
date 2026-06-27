# Análise de Preferências Musicais - Springfield vs Shelbyville

> Projeto de análise de dados de um serviço de streaming de música para comparar o comportamento dos usuários das cidades de Springfield e Shelbyville, testando a hipótese de que a atividade dos usuários é diferente dependendo do dia da semana e da cidade.

---

## 🎯 Objetivo do Projeto

Testar a seguinte hipótese:

**Hipótese:** A atividade dos usuários é diferente dependendo do dia da semana e da cidade.

Para isso, foram analisados dados de um serviço de streaming de música online, comparando o comportamento dos usuários de Springfield e Shelbyville em três dias específicos: segunda-feira (Monday), quarta-feira (Wednesday) e sexta-feira (Friday).

---

## 📊 Resultados Obtidos

### Principais descobertas:

- **Springfield** tem mais que o dobro de músicas reproduzidas em comparação com Shelbyville em todos os dias analisados.
  - Springfield: **42.741** músicas
  - Shelbyville: **18.512** músicas

- **Padrão de comportamento por dia:**
  - **Springfield:** maior consumo na **sexta-feira** (15.945) e **segunda-feira** (15.740)
  - **Shelbyville:** maior consumo na **quarta-feira** (7.003)

| Cidade | Segunda-feira | Quarta-feira | Sexta-feira |
|--------|---------------|--------------|-------------|
| Springfield | 15.740 | 11.056 | 15.945 |
| Shelbyville | 5.614 | 7.003 | 5.895 |

### Conclusão da hipótese:

✅ **A hipótese foi confirmada.** A atividade dos usuários é diferente dependendo do dia da semana e da cidade.

- Springfield apresenta picos de consumo às segundas e sextas-feiras.
- Shelbyville apresenta seu pico de consumo às quartas-feiras.
- Springfield tem uma base de usuários significativamente maior (mais que o dobro) em comparação com Shelbyville.

---

## 🛠️ Ferramentas Utilizadas

- **Python 3**
- **Bibliotecas:**
  - `pandas` — para manipulação e análise de dados
  - Nenhuma biblioteca externa adicional foi necessária

---

## 📚 O que Aprendi

- **Leitura e análise inicial de dados:** uso de `pd.read_csv()` e `df.info()` para entender a estrutura dos dados
- **Limpeza de cabeçalhos:** padronização de nomes de colunas (lowercase, remoção de espaços, substituição de caracteres)
- **Tratamento de valores ausentes:** substituição de valores nulos por `'unknown'` utilizando `.fillna()`
- **Remoção de duplicados explícitos:** uso de `.drop_duplicates()` para eliminar linhas duplicadas
- **Correção de duplicados implícitos:** criação de função para padronizar gêneros musicais (ex: `hip`, `hop`, `hip-hop` → `hiphop`)
- **Agrupamento e agregação:** uso de `.groupby()` para contar músicas por cidade e por dia
- **Criação de funções personalizadas:** desenvolvimento da função `number_tracks(day, city)` para filtragem e contagem simultânea
- **Teste de hipóteses:** análise comparativa de comportamento de usuários entre cidades

---

## 🚀 Como Executar o Projeto

```bash
# Clone o repositório
git clone https://github.com/LuizAlmeida/analise_preferencias_musicais_springfield_shelbyville

# Navegue até a pasta do projeto
cd analise_preferencias_musicais_springfield_shelbyville

# Execute o notebook (recomendado: Google Colab ou Jupyter Notebook)
# Ou execute o script Python diretamente
python analise_musica.py
````

## Requisitos:
- Python 3.x instalado
- Jupyter Notebook (opcional) ou Google Colab (recomendado)
- Biblioteca pandas instalada: pip install pandas


## 🔍 Metodologia
O projeto seguiu uma abordagem estruturada em 3 etapas:


## Etapa 1: Visão Geral dos Dados
- Leitura do arquivo CSV
- Análise da estrutura e tipos de dados
- Identificação de problemas nos cabeçalhos e valores ausentes


## Etapa 2: Pré-processamento de Dados
- Padronização de cabeçalhos (lowercase, remoção de espaços)
- Correção do nome da coluna userid → user_id
- Substituição de valores ausentes em track, artist e genre por 'unknown'
- Remoção de duplicados explícitos (3.826 linhas removidas)
- Correção de duplicados implícitos no gênero hiphop (agrupando hip, hop e hip-hop)


## Etapa 3: Teste da Hipótese
- Contagem de músicas por cidade
- Contagem de músicas por dia da semana (segunda, quarta e sexta)
- Criação da função number_tracks(day, city) para análise cruzada
- Comparação dos resultados entre cidades


## 💡 Melhorias Futuras
- Realizar testes estatísticos para validar as diferenças observadas (ex: teste t ou qui-quadrado)
- Analisar os gêneros musicais mais ouvidos em cada cidade para entender preferências culturais
- Identificar os artistas mais tocados em cada cidade
- Criar visualizações gráficas (gráficos de barras, heatmaps) para facilitar a interpretação dos dados
- Analisar dados de outros dias da semana para um comparativo completo
- Investigar possíveis correlações entre idade dos usuários e preferências musicais


## 📁 Estrutura do Projeto
````
📁 analise_preferencias_musicais_springfield_shelbyville/
├── 📁 datasets/                    # Dados utilizados
│   └── music_project_en.csv
├── 📁 notebooks/                   # Notebook Jupyter com análise completa
│   └── Projeto_Sprint_2.ipynb
├── 📁 scripts/                     # Scripts Python avulsos
├── README.md                       # Este arquivo
└── requirements.txt                # Dependências do projeto
````


## 📌 Contato
- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/luizmarques84)
- [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LuizAlmeida)


## ⭐ Este projeto faz parte do meu Bootcamp em Análise de Dados na TripleTen.
````

---

## 🎯 RESUMO DO QUE FAZER

| Ação | Status |
|------|--------|
| Criar repositório `analise_preferencias_musicais_springfield_shelbyville` | ⬜ |
| Fazer upload do arquivo `.ipynb` | ⬜ |
| Adicionar README.md com o texto acima | ⬜ |
| Adicionar tópico `tripleten` | ⬜ |
| Fixar (pinned) no perfil | ⬜ |

---

Me avise quando terminar e passamos para o **Sprint 3**! 🚀
````


