# Projeto Integrado - Vitrine e FAQ Dinâmico (Shakers) 

## 📋 Descrição do Projeto
Este projeto consiste no desenvolvimento de uma vitrine funcional dentro da plataforma Shopify[cite: 9]. [cite_start]A solução foca na criação de componentes reutilizáveis (sections), uso de objetos da plataforma e renderização de dados dinâmicos através de Metafields na página de produto.

## 🛠️ O que foi implementado
* **Home Page:**
    * Hero Slider configurável (Título, Texto, Botão, Imagem).
    * Listagem de produtos de uma coleção selecionada via schema.
    *Botão de Call to Action (CTA) final
* **Página de Produto (PDP):**
    * Renderização modular de informações (Título, Preço, Descrição).
    * Sistema de seleção de variantes e botão "Add to Cart" funcional via JS.
    * Seção de FAQ dinâmica alimentada por Metafields de Metaobjetos.

##🚀 Como testar localmente com Shopify CLI 
1. Clone o repositório:
   `git clone https://github.com/BORGES-GRU/shakers-projeto-integrado-vitrine-faq.git`
2. Acesse a branch de desenvolvimento:
   `git checkout feat/projeto-integrado-vitrine-faq` 
3. Autentique-se na sua loja:
   `shopify login --store sua-loja-teste.myshopify.com`
4. Inicie o servidor local:
   `shopify theme dev`

## ⚙️ Configurações no Shopify Admin 
1. **Home Page:** No editor de temas, adicione as seções `Hero Slider`, `Collection Product List` e `Final CTA` para configurar os conteúdos.
2. **Criar Metaobjeto de FAQ:** 
    * Vá em **Configurações > Dados Personalizados > Metaobjetos**.
    * Crie o metaobjeto `faq_item` com os campos `pergunta` (single line text) e `resposta` (multi-line text).
3. **Criar Metafield e Associar ao Produto:** 
    * Vá em **Configurações > Dados Personalizados > Produtos**.
    * Crie um campo chamado `FAQ List`, selecione o tipo **Metaobject** e marque **"Lista de entradas"**, referenciando o `faq_item`.
    *No cadastro do produto, adicione pelo menos 3 entradas de FAQ.

## 🔗 Links 
* **Pull Request:** https://github.com/BORGES-GRU/shakers-projeto-integrado-vitrine-faq/pull/1
* **Vídeo de Apresentação:** https://drive.google.com/file/d/1GBqBpFEKtXfIyi0xMnVLa9LCcnDpkgLn/view?usp=sharing
