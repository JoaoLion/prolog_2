# prolog_2
Atividade 7 - Lab Guiado Prolog (2)


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
