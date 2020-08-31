# MWE_MarkovChain

Modelos de linguagem servem de base para uma série de tarefas de processamento de linguagem natural, entre elas a geração automática de textos.  Em muitos casos as palavras são usadas como tokens, ou seja, como unidades básicas para o processamento do texto. Para documentos de domínios específicos, onde existem muitas expressões e jargões próprios, as expressões multipalavras (ou multiword expressions) podem impactar no processamento dos texto. Buscando subsidiar a construção de modelos de linguagem, neste trabalho avaliamos o impacto das expressões multipalavras na criação destes modelos.  Criamos dois modelos de linguagem estatísticos usando Cadeias de Markov, o primeiro utilizou apenas palavras únicas como tokens, já o segundo modelo juntou as expressões multipalavras em um token único. As expressões multipalavras do segundo modelo foram identificadas usando a métrica Informação Mútua (Mutual Information). Por fim, comparamos os dois modelos avaliando as suas perplexidades.

Após os nossos testes, encontramos que o modelo que utilizou apenas palavras únicas teve o melhor resultado. Portanto, considerar as expressões multipalavras não melhorou os modelos de linguagem de domínio específico. Esse trabalho foi limitado a modelos de linguagem estocástico, portanto é necessário avaliar se os mesmos resultados se mantém para modelos baseados em redes neurais. Também é importante avaliar o comportamento dos modelos de linguagem ao usar subpalavras - tokenização de elemento com tamanho inferior ao tamanho das palavras.