| NOME DO CAMPO | PROPRIEDADE JSON |TIPO |        | MÁXIMO DE CARACTERES	|ACEITA VALORES NULOS |DESCRIÇÃO	| OBSERVAÇÕES|
|---------------| ---------------- |---- |--------|------------ |-------------------- |-------------------- |--------------------------------- |
| NUMERO_PEDIDO_SUPPLIER | order_id|text| Livre |	N/A	|Não|	Número do pedido do serviço contratado pelo cliente Allpoints||
| PEDIDO_DATA            | order_time  |datetimeoffset| ISO 8601 YYYY-MM-DDThh:mm:ss.sTZD (eg 1997-07-16T19:20:30.45+01:00)	|N/A	|Não	|Data da compra	||
|VIAGEM_CHECKIN	|travel_check_in_time	|datetimeoffset	| ISO 8601 YYYY-MM-DDThh:mm:ss.sTZD (eg 1997-07-16T19:20:30.45+01:00)|	N/A	|Sim	|Data e horário do início da utilização do serviço contratado	||
|VIAGEM_CHECKOUT|	travel_check_out_time	|datetimeoffset	 |ISO 8601 YYYY-MM-DDThh:mm:ss.sTZD (eg 1997-07-16T19:20:30.45+01:00)	|N/A	|Sim	|Data e horário do final da utilização do serviço contratado|	|
|VIAGEM_SITUACAO|	travel_status|	text|	Livre|	100	|Não	|Indicação da situação da VIAGEM	|Devemos receber apenas pedidos com CHECK OUTS concluídos|
|CLIENTE_NOME	|customer_name	|text	|Livre|	11	|Sim	|Nome do cliente contratante do serviço	||
|CLIENTE_DOCUMENTO_NUMERO	|customer_legal_id_number	|text	|Somente números e letras	|100	|Não|	Documento do cliente estrangeiro (CPF; Passaporte, RNE)|	Para brasileiros, a chave de cadastro e pontuação no Programa Allpoints deve ser o CPF|
|CLIENTE_DOCUMENTO_TIPO	|customer_legal_id_type|	text|	Livre|	100|	Não	|Tipo do documento do cliente estrangeiro (CPF, Passaporte, RNE, etc)	||
|CLIENTE_EMAIL |customer_email	|	text|	E-mail válido|	30|	Não	|E-mail do cliente||
|CLIENTE_CELULAR	|customer_phone_number|	text	|Número de telefoneválido com código do país	|100|Não	|Celular do cliente com DDD e DDI||
|CLIENTE_PAIS	|customer_country	|text	|Livre	|100	|Sim	|País de endereço do cliente	||
|HOSPEDE_CIDADE	|customer_city|	text	|Livre	|100	|Sim	|Cidade de endereço do cliente|	|
|CLIENTE_UF|	customer_state|	text|	Livre|	100|	Sim	|Estado de endereço do cliente|	Apenas dois valores possíveis: "PRINCIPAL" e "ACOMPANHANTE"|
|VALOR_PEDIDO|	order_value|	number|	Livre	|30	|Não	|Valor pago pelo serviço contratado	|Formato de valor monetário "0,00"|
|CAMPANHA_ALLPOINTS|	campaign_id|	text	|Livre	|30	|Não	|Código da campanha de pontuação vigente	|Código fornecido previamente pela Allpoints de acordo com possíveis campanhas|
|SIGN_IN_FIDELIDADE	|loyalty_opt_in	|boolean	| boolean	|30	|Não|	Autorização do cliente para participação do Programa de Fidelidade Allpoints (Sim ou Não)|	A autorização deve ser concedida pelo cliente no momento da contratação do serviço|
|SIGN_IN_FIDELIDADE_DATE|	loyalty_opt_in_time|	datetimeoffset	| ISO 8601 YYYY-MM-DDThh:mm:ss.sTZD (eg 1997-07-16T19:20:30.45+01:00)|	N/A	|Não|	Data da autorização do hóspede para participação do Programa de Fidelidade Allpoints|

