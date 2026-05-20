# prolog_2
Atividade 7 - Lab Guiado Prolog (2)

## Codigo
![Descrição](prolog/codigo.png)

## Parte 3
Passo 3.1: Vamos perguntar ao Prolog qual é a melhor cor para a Mesa 1.   
PERGUNTA 1: Qual foi a cor recomendada?. Tinto  

Passo 3.2: Vamos perguntar o tipo de vinho.  
PERGUNTA 2: Qual foi o tipo recomendado?. Seco  

Passo 3.3 (A Pergunta de Ouro): Vamos pedir para a máquina cruzar tudo e dar a sugestão final.  
PERGUNTA 3: Qual foi o vinho exato que o sistema recomendou?  
V = cabernet_sauvignon  
PERGUNTA 4 Explique com as suas próprias palavras como o Prolog chegou sozinho a essa conclusão matemática (como ele encadeou as regras). 
Resposta: O Prolog analisou os fatos do cliente: prato_principal(massa). molho(tomate)., Como o prato era massa, a regra definiu a cor como tinto, o molho era tomate, a regra definiu o tipo como seco.
Em seguida, o Prolog procurou um vinho que fosse ao mesmo tempo tinto e seco. A regra do cabernet_sauvignon dizia exatamente isso.




% Regras de Cor
melhor_cor(tinto) :- prato_principal(carne_vermelha) ; prato_principal(massa).
melhor_cor(branco) :- prato_principal(frango) ; prato_principal(peixe).
% melhor_cor(branco) :- prato_principal(salada).

% Regras de Tipo
melhor_tipo(suave) :- molho(sem_molho) ; molho(picante).
melhor_tipo(seco) :- molho(tomate).% ; molho(ervas).

% Regras de Vinho
melhor_vinho(cabernet_sauvignon) :- melhor_cor(tinto) , melhor_tipo(seco).
melhor_vinho(pinot_noir) :- melhor_cor(tinto) , melhor_tipo(suave).
melhor_vinho(riesling) :- melhor_cor(branco) , melhor_tipo(suave).

% Pedido do Cliente
prato_principal(massa).
molho(tomate).



melhor_cor(branco) :- prato_principal(salada).

melhor_tipo(seco) :- molho(ervas).


melhor_vinho(chardonnay) :-
    melhor_cor(branco),
    melhor_tipo(seco).
