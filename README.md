# prolog_2
Atividade 7 - Lab Guiado Prolog (2)

## Codigo
![Descrição](prolog2/codigo_1.png)

## Parte 3
Passo 3.1: Vamos perguntar ao Prolog qual é a melhor cor para a Mesa 1.   
PERGUNTA 1: Qual foi a cor recomendada?. Tinto  
![Descrição](prolog2/tinto.png)

## Passo 3.2: Vamos perguntar o tipo de vinho.  
PERGUNTA 2: Qual foi o tipo recomendado?. Seco  
![Descrição](prolog2/seco.png)

## Passo 3.3 (A Pergunta de Ouro): Vamos pedir para a máquina cruzar tudo e dar a sugestão final.  
PERGUNTA 3: Qual foi o vinho exato que o sistema recomendou?  
V = cabernet_sauvignon  
![Descrição](prolog2/vinho1.png)

## PERGUNTA 4 Explique com as suas próprias palavras como o Prolog chegou sozinho a essa conclusão matemática (como ele encadeou as regras). 
Resposta: O Prolog analisou os fatos do cliente: prato_principal(massa). molho(tomate)., Como o prato era massa, a regra definiu a cor como tinto, o molho era tomate, a regra definiu o tipo como seco.
Em seguida, o Prolog procurou um vinho que fosse ao mesmo tempo tinto e seco. A regra do cabernet_sauvignon dizia exatamente isso.


## PARTE 4: MISSÕES INDEPENDENTES

Desafio 1: O Cliente Vegano
O restaurante agora serve Salada. A regra é: "Se o prato for salada, a melhor cor é branco." Além disso, criaram um molho de Ervas Finais. A regra é: "Se o molho for de ervas, o vinho deve ser seco."
Missão: Adicione essas regras, troque o pedido do cliente para prato_principal(salada). e molho(ervas). e rode a consulta melhor_vinho(V). Qual vinho o sistema recomendou para o vegano?
V = False

🕵️ Desafio 2: O Novo Vinho
A adega acaba de receber garrafas de Chardonnay. O Sommelier determinou que esse vinho é recomendado apenas quando a melhor cor for Branco e o melhor tipo for Seco.
