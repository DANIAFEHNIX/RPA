# RPA
Testes de Robô em planilha excel
Objetivo:

Cada arquivo possui uma coluna chamada “DOCUMENTO” este é o número do documento que será utilizado como chave para fazer referência entre os arquivos.

O script deve realizar a leitura do arquivo de REMESSA_BANCARIA.xlsx , e para cada número de documento lido deverá localizar o documento referente no arquivo RETORNO_BANCARIO.xlsx. 
Para cada número de documento lido deverá ser:
* Comparado às coluna de data de vencimento e data de pagamento se há divergência entre elas. Caso houver atraso no pagamento deverá ser verificado se o valor pago foi aplicado os juros que estavam previstos no arquivo de remessa na coluna “% JUROS POR ATRASO”. Caso não tenha sido aplicado os juros registrar a mensagem na coluna OBSERVAÇÃO, “ PAGAMENTO EM ATRASO COM VALOR DIVERGENTE”
*Se a coluna VALOR estiver em branco significa que não houve pagamento ainda. Deverá ser verificado se está em atraso ou se está dentro do prazo de vencimento. Se estiver em atraso registrar a mensagem na coluna OBSERVAÇÃO, “PAGAMENTO EM ATRASO”.
*Se o pagamento foi realizado dentro do prazo de vencimento, verificar se o valor pago é igual ao valor que teria que ser pago, se valor for divergente registrar a mensagem na coluna OBSERVAÇÃO, “PAGAMENTO COM VALOR DIVERGENTE”.
