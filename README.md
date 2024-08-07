# Cardapio_Ifruit

O código começa com a sintaxe HTML. HTML define a estrutura de uma página web. Aqui está uma análise dos elementos principais:

<!DOCTYPE html>: Esta declaração define o tipo de documento como HTML.
<html>: O elemento raiz do documento HTML.
<head>: Esta seção contém meta informações sobre o documento, como codificação de caracteres e o título da página.
<meta charset="UTF-8">: Especifica a codificação de caracteres (UTF-8 para a maioria dos sites modernos).
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Define a viewport para design responsivo, garantindo que a página se adapte a diferentes tamanhos de tela.
<title>Cardápio Digital</title>: Define o título da página web, que será exibido na aba do navegador.
<style>: Esta seção contém código CSS que define o estilo dos elementos HTML. Aqui, ele define estilos para fontes, cores de fundo, layout e muito mais.
<body>: Esta seção contém o conteúdo visível da página web.

header: Esta seção cria um elemento de cabeçalho com o nome do restaurante ("Cardápio Digital - IFruit").
div.container: Envolve a maior parte do conteúdo dentro de um contêiner (div) com a classe "container" para melhor organização e layout responsivo (opcional).
div.cardapio: Esta seção representa o menu em si. Ele contém várias categorias de itens alimentares (div.categoria).
div.categoria: Cada categoria (por exemplo, Hambúrgueres, Salgados, Bebidas) é encapsulada em uma div com a classe "categoria" e inclui um título (<h2>).
div.item: Cada item alimentar é exibido dentro de uma div com a classe "item". Ele usa uma combinação de elementos HTML para estruturar o conteúdo:
<input type="checkbox">: Caixas de seleção permitem que os usuários escolham os itens que desejam pedir.
<label for="checkboxId">: As etiquetas estão associadas às caixas de seleção usando o atributo for para fornecer texto descritivo ao lado de cada caixa de seleção.
<span class="descricao">: Spans com a classe "descricao" exibem informações adicionais sobre o item alimentar.
<input type="number" class="quantidade">: Campos de entrada numéricos permitem que os usuários especifiquem a quantidade de cada item selecionado. Eles estão inicialmente desabilitados e se tornam habilitados quando a caixa de seleção correspondente é marcada.
div.carrinho: Esta seção representa o carrinho de compras.
<h2>Carrinho de Compras</h2>: Título para o carrinho de compras.
table: Uma tabela exibe os itens selecionados, quantidade e preço.
thead: O cabeçalho da tabela (thead) define as colunas da tabela: Item, Quantidade, Preço.
tbody#carrinho-itens: O corpo da tabela (tbody) com o ID "carrinho-itens" é onde as linhas para cada item selecionado serão adicionadas dinamicamente usando JavaScript.
div.total: Exibe o preço total dos itens selecionados. Ele usa um span com o ID "total" para atualizar o valor dinamicamente.
div.pagamento: Seção para selecionar o método de pagamento. Ele usa botões de rádio para permitir que os usuários escolham entre Dinheiro, PIX ou Cartão.
div.endereco: Seção para inserir o endereço de entrega. Inclui um rótulo (<h3>) e uma área de texto (textarea) para o usuário inserir seu endereço.
button.finalizar: Dois botões com a classe "finalizar" são exibidos. Potencialmente, um é para finalizar o pedido, enquanto o outro pode ser para cancelá-lo

O script seleciona todas as caixas de seleção usando querySelectorAll('input[type="checkbox"]') e as atribui à constante checkboxes.
Ele também seleciona o elemento do corpo da tabela com o ID "carrinho-itens" e o atribui à constante carrinhoItens.
