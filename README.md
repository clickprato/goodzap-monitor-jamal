# v.1.14.1 - CP-Aut9/interface-gallery-desk - 22/11/2026

vAMOS AVANÇAR PARA A PRóXIMA ETAPA: cRIE UMA ABA CHAMADA "cAMPANHAS"dentro da pagina "goodzap", entre "configuraçÕes gerais" e "sistema". Essa aba devera conter os campos "Nome da PromoçÃo", "Regras" e "Validade da PromoçÃo". A data da validade deve ser salva no formato dd/mm/aaaa. Esses campos devem ter opçÕes CRUD, e devo poder adicionar mais de uma promocao com os mesmos campos e todas podem ser ativadas ou desativadas. Teremos algum problema para implantar?

Hoje às 03:48



Planejando os campos das campanhas
Faltaram duas coisas que nao tÊm no projeto original: cada promocao deve ter um campo chamado "UTM da PromoçÃo" e na aba "SISTEMA", um novo campo chamado "URL do Cardápio"

Hoje às 03:54


Confirmou os dois campos extras
Anotado: incluo "UTM da Promoção" em cada promoção e "URL do Cardápio" na aba Sistema junto com a aba Campanhas.

Criou a aba Campanhas e o campo URL do Cardápio
Não tivemos nenhum problema. A página GoodZap agora tem a aba Campanhas, entre Configurações Gerais e Sistema. Nela você pode adicionar quantas promoções quiser, cada uma com Nome da Promoção, Regras, Validade da Promoção (dd/mm/aaaa) e UTM da Promoção. Dá para editar e excluir cada uma, e ativar ou desativar com a chave.

Na aba Sistema apareceu o campo URL do Cardápio (só super-admin vê). Tudo isso já chega ao n8n pela mesma consulta que você usa hoje.

Três observações:

A validade é guardada exatamente como dd/mm/aaaa. Datas inválidas, como 31/02, são recusadas.
As promoções que você já tinha saíram de Configurações Gerais e agora ficam só em Campanhas.
Testei as regras da data, mas não abri a página com login para ver na tela. Vale cadastrar uma promoção para conferir.
Mudei a forma como a data de validade é guardada, então publique o app para a versão no ar continuar funcionando. Se usa o projeto clonado, rode lá também a atualização dos novos campos. Posso te passar esse trecho se quiser.
