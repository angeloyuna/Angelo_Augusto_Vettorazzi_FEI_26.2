# Projeto 1 - Loja Virtual: Estrutura e Interface (HTML e CSS)

## Descrição da Loja

A loja ficcional Enna's Fishing Wares é uma empresa que possui o objetivo de oferecer apoio às comunidades de pescaria presentes no mundo ficcional em que habita, através do seu estabelecimento físico e também pelo seu site, que foi criado nesse projeto.

Através de seis páginas .html e quatro documentos .css, a loja virtual oferece:

- Página inicial com produtos destacados e uma descrição da loja, com imagens presentes para a descrição e os produtos
- Loja com sessão de catálogo, que possui uma barra de pesquisa e múltiplos tipos de filtros que podem ser aplicados, e uma sessão de carrinho e finalização da compra
- Formulário de cadastro para usuários cadastrarem suas contas
- Formulário de login para usuários entrarem em suas contas
- Página de perfil contendo os pedidos do usuário conectado, além de um formulário para editar seus dados
- Página exclusiva para administradores verificarem os relatórios das compras e clientes da loja, incluindo barras de pesquisa com opções do modo de pesquisa, além de um template único quando a página for imprimida 
- Informações da empresa e formulário para contatar a loja presente no rodapé de todas as páginas
- Responsividade com resoluções de desktop (Comprimento de 1920px, 1600px, 1280px) tablet (Comprimento de 840px) e smartphone (Comprimento de 320px)

## Integrantes

- Angelo Augusto Vettorazzi [(angeloyuna)](https://github.com/angeloyuna)

## Estrutura de pastas

- [html/](html/)
  - index.html
  - loja.html
  - cadastro.html
  - login.html
  - perfil.html
  - relatorios.html
- [css/](css/)
  - base.css
  - componentes.css
  - relatorios.css
  - responsivo.css
- [img/](img/)
  - lojaFisicaExterior.png
  - lojaFisicaInterior.png
  - [header/](header/)
    - logo.png
    - menu.png
  - [produtos/](produtos/)
    - anzolCircleHook.png
    - anzolMaruseigo.png
    - carretilhaAlto.png
    - carretilhaBaixo.png
    - iscaFundo.png
    - iscaMeiaAgua.png
    - iscaSuperficie.png
    - linhaMonofilamento.png
    - linhaMultifilamento.png
    - molineteL.png
    - molineteUL.png
    - varaL.png
    - varaM.png
    - varaML.png
    - varaUL.png

<!-- Necessário adicionar seção contendo instruções para a visualização de telas ocultas !-->

## Visualização de Telas e Elementos Ocultos

Como este projeto ainda não possui integração com a linguagem de JavaScript, a loja possui elementos e telas são inacessíveis sem a alteração direta do código ou consciência de todos os documentos .html que fazem parte do website. Logo, essa seção tem o objetivo de demonstrar como acessar essas telas e elementos ocultos

### Elementos Ocultos

<ins>Compra Finalizada e Número de Pedido em loja.html</ins>

Para acessar estes elementos presentes na seção de Carrinho no documento [loja.html](html/loja.html), é necessário remover o atributo `hidden` presente na linha 358 do mesmo documento:

<b>Antes</b>

```html
<div hidden id="carrinho-compra-finalizada">
  <p>Compra Finalizada!</p>
  <p>Número de Pedido: CP001</p>
</div>
```

<b>Depois</b>

```html
<div id="carrinho-compra-finalizada">
  <p>Compra Finalizada!</p>
  <p>Número de Pedido: CP001</p>
</div>
```

### Telas Ocultas

<ins>perfil.html e relatorios.html</ins>

Como estes documentos necessitam de um usúario conectado a uma conta para acessarem eles, a falta de integração com um sistema de usuário funcionável faz com que acessar esses documentos, através da página inicial [index.html](html/index.html) e os outros documentos acessíveis através dela, necessite uma mudança direta da URL da página do navegador que está acessando o site. Esse processo de mudar a URL é feito dessa forma:

<b>Antes</b> (index.html é apenas um exemplo, essa mudança não necessita começar nesse documento)

```
../Angelo_Augusto_Vettorazzi_FEI_26.2/html/index.html
```

<b>Depois</b>

```
../Angelo_Augusto_Vettorazzi_FEI_26.2/html/perfil.html
../Angelo_Augusto_Vettorazzi_FEI_26.2/html/relatorios.html
```
