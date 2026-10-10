# tcc-uwine-ciencia-de-dados
TCC em Ciência de Dados (UVV) — análise estatística e Machine Learning sobre dados simulados do UWine, clube de vinhos universitário fictício.

# UWine: Quantos dados bastam? (Parte 1)

Trabalho de Conclusão de Curso em Ciência de Dados (Universidade Vila Velha). Análise estatística do UWine, um clube de vinhos universitário fictício, com 1,12 milhão de notas fiscais simuladas e 23 variáveis.

**Vídeo de apresentação:** https://www.youtube.com/watch?v=2plNuetyDpc

## O que este projeto responde

Antes de aplicar Machine Learning (Parte 2), qual tamanho de amostra representa bem cada tipo de conta (ESSENTIAL, VIP e PRIME), sem viés e com confiança comprovada?

## Principais resultados

| Etapa | Resultado |
|---|---|
| Tamanho de amostra adotado | 40.000 observações por tipo de conta |
| Funções do professor (parâmetros padrão) | Empírica: 14.200 a 30.700 por grupo. Teórico-empírica (Neyman): 5.300 no total |
| Busca por bootstrap (margem do IC de 95% de até 1%) | VIP 10.000, PRIME 15.000, ESSENTIAL 25.000, geral 40.000 |
| Validação com n = 40.000 | Viés abaixo de 0,02%, margem entre ±0,48% e ±1,00%, cobertura do IC entre 95% e 97% |
| Outliers (IQR, por grupo) | ESSENTIAL 3,66%, VIP 2,71%, PRIME ~0%. Todos mantidos |
| Testes ESSENTIAL x PRIME | Não normais, independentes, distribuições e médias diferentes |
| Satisfação | 77% satisfeitos, nota média 3,77 (IC 95%: 3,76 a 3,78), sem diferença por sexo |

## Conteúdo do repositório

- `MarcioJr_PARTE_1.ipynb`: notebook com todo o código e os resultados.

## Como reproduzir

1. Abra o notebook no Google Colab.
2. Envie o arquivo `table45.csv` para a sessão do Colab (ou monte o Google Drive).
3. Execute as células em ordem.

O arquivo de dados (cerca de 400 MB) não está neste repositório porque excede o limite de 100 MB do GitHub. A base é simulada e foi fornecida pela universidade.

## Ferramentas

Python, pandas, NumPy, SciPy, Matplotlib e Seaborn.

## Autor

Marcio Ferreira dos Santos Junior
