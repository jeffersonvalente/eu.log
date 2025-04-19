# 007 — Silêncio antes do incidente

No início, a gente só sabia que algo tinha dado errado… quando já tava dando muito errado.

Era usuário reclamando que o site caiu.  
Era analista perguntando por que o serviço parou.  
Era SLA estourando no susto.

A gente vivia correndo atrás do rastro.

Foi aí que eu mergulhei de vez no Zabbix.

Comecei pelas bases: configurar host, coletar métricas, ajustar triggers.  
Mas logo entendi que, se só mostrasse consumo de CPU, eu ia estar só pintando gráfico bonito.  
Então foquei no que realmente ajudava o time:

- alertas com contexto, não só número
- agrupamento por criticidade e impacto
- thresholds adaptados à realidade da infra, não ao default da ferramenta

Montei templates que viraram base pra novos serviços.  
Reduzi falsos positivos.  
E, pela primeira vez, vi um alerta disparar **antes** de alguém abrir um chamado.

Lembro de um em especial:  
um banco de dados começava a travar por uso de disco no temp.  
O alerta disparou quando ainda dava tempo de agir.

A gente entrou, limpou, ajustou.  
O cliente final nem ficou sabendo.

E eu fiquei ali olhando o gráfico voltar pro normal,  
sabendo que, dessa vez, a gente chegou antes.

Não teve aplauso.  
Mas também não teve incidente.

E às vezes, no mundo da infraestrutura,  
**o silêncio é o sinal de que você acertou.**
