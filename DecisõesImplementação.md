# Decisões de Implementação

## Índice Invertido

A implementação escolhida para o índice invertido foi: dicionário no qual a chave é um termo/token resultante do pré-processamento e o valor é também um dicionário, sendo nesse caso o par chave-valor representado pelo ID do documento em que o token está presente e pela quantidade de aparições do token no documento. A partir disso, obtemos uma leitura em O(1) tanto para o termo quanto para o document ID, o que é relevante, considerando que diversas queries serão realizadas para posterior análise. Além disso, no momento da criação do índice, em comparação com uma abordagem em array ou lista, não há o custo de ordenação de tokens (O(nlogn)), permitindo uma build mais rápida.

Vale destacar ainda que o custo de armazenamento (O(n * m), onde n é o número de tokens e m é o número de documentos em cada dicionário de token) não é, considerando o dataset atual e considerando que, a cada novo índice invertido criado, o anterior será liberado, uma limitação.