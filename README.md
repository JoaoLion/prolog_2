# prolog_2
Atividade 7 - Lab Guiado Prolog (2)

## Codigo
![Descrição](prolog2/codigo_1.png)

## Parte 3
Passo 3.1: Vamos perguntar ao Prolog qual é a melhor cor para a Mesa 1.   
PERGUNTA 1: Qual foi a cor recomendada?. Tinto  
![Descrição](prolog2/tinto.png)

Passo 3.2: Vamos perguntar o tipo de vinho.  
PERGUNTA 2: Qual foi o tipo recomendado?. Seco  
![Descrição](prolog2/seco.png)

Passo 3.3 (A Pergunta de Ouro): Vamos pedir para a máquina cruzar tudo e dar a sugestão final.  
PERGUNTA 3: Qual foi o vinho exato que o sistema recomendou?  
V = cabernet_sauvignon  
![Descrição](vinho2/tinto.png)

PERGUNTA 4 Explique com as suas próprias palavras como o Prolog chegou sozinho a essa conclusão matemática (como ele encadeou as regras). 
Resposta: O Prolog analisou os fatos do cliente: prato_principal(massa). molho(tomate)., Como o prato era massa, a regra definiu a cor como tinto, o molho era tomate, a regra definiu o tipo como seco.
Em seguida, o Prolog procurou um vinho que fosse ao mesmo tempo tinto e seco. A regra do cabernet_sauvignon dizia exatamente isso.


## PARTE 4: MISSÕES INDEPENDENTES
