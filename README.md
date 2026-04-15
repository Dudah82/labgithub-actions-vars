## Desafio Prático: Dominando Variáveis e Escopos no GitHub Actions.

### Perguntas de reflexão:

• Por que a Secret aparece no log como ** e a variável aparece normalmente?

R= Pois a Secret serve justamente para guardar dados sensíveis como senhas e tokens, ao tentar imprimir essa variável o GitHub a esconde para evitar que alguém que veja seus logs consiga roubar senhas e chaves importantes. Já a viriável, é para coisas comuns como URL da API por exemplo, então o GitHub exibi ela normalmente, em texto limpo.

• O Job deploy_app consegue ler a variável BUILD_VERSION criada no Job build_app? Por quê?

R= Não, pois como ela foi definida dentro daquele job específico (build_app) ela só pode ser usada nele, sendo assim ela se torna invisível para os outros jobs.


