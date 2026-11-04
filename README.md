# 🍷 Vinasco Closet (High Fashion MVP)

Desafio de projeto da **DIO (Digital Innovation One)** para criação de um MVP de e-commerce e agendamento de atendimento exclusivo para moda autoral utilizando o conceito de **Vibe Coding** com o auxílio do **Copilot Web** e do **Lovable**.

🔗 **[Acesse a Aplicação Publicada Aqui](https://preview--pixel-perfect-playback-3778.lovable.app/?__lovable_receipt=mat_0pev5ep0m6898s7t1nkqfh25qa)**

---

## 🎯 1. A Dor Escolhida e Por Que Vale um Negócio

- **A Dor Escolhida:** Lojas de moda independentes, boutiques autorais e closets digitais sofrem para organizar pedidos sob medida, expor coleções exclusivas de forma elegante e realizar a triagem de clientes sem depender de estruturas complexas e caras de e-commerce logo no início.
- **Por que vale um negócio:** O mercado de moda autoral valoriza a exclusividade e o atendimento intimista. Automatizar a vitrine digital enquanto mantém a relação consultiva e direta com o cliente gera alta conversão e fidelização com baixo custo operacional inicial.

---

## 📊 2. Tamanho de Mercado e Business Model Canvas

### Tamanho de Mercado
- **TAM (Total Addressable Market):** Mercado nacional de vestuário, alta costura e e-commerce de moda independente.
- **SAM (Serviceable Available Market):** Consumidoras de moda autoral e marcas independentes ativas nas redes sociais.
- **SOM (Serviceable Obtainable Market):** As primeiras dezenas de clientes recorrentes engajadas e captadas organicamente pela marca.

### Business Model Canvas (Resumo)
* **Parceiros-Chave:** Fornecedores de tecidos/peças e serviços de entrega (Correios/motoboy).
* **Atividades-Chave:** Curadoria de peças, atendimento humanizado e gestão de pedidos.
* **Recursos-Chave:** Vitrine digital (MVP), Instagram da marca e WhatsApp para atendimento.
* **Proposta de Valor:** Peças exclusivas de alta qualidade com atendimento consultivo e exclusivo (estilo closet privado).
* **Relação com o Cliente:** Direta, empática e consultiva via WhatsApp.
* **Canais:** Instagram, Indicações e a Landing Page do MVP.
* **Segmento de Clientes:** Mulheres que buscam estilo autêntico, peças limitadas e atendimento personalizado.
* **Estrutura de Custos:** Aquisição de coleções de vestuário e hospedagem da aplicação.
* **Fontes de Receita:** Venda direta das peças de vestuário e kits de looks exclusivos.

---

## 🧪 3. A Tese do MVP e O Que Ficou Manual

- **A Tese do MVP:** Clientes de moda autoral preferem navegar por uma vitrine visualmente refinada (com estética de alta costura) e preferem alinhar os detalhes, tamanhos e ajustes diretamente através de um atendimento humanizado e ágil no WhatsApp.
- **O que ficou manual de propósito:** 
  - **Pagamento:** Sem gateway integrado (como Stripe ou Mercado Pago). O fechamento financeiro, envio de Pix ou link de pagamento avulso ocorrem manualmente na conversa do WhatsApp.
  - **Controle de Estoque:** Atualizado manualmente no painel administrativo conforme a confirmação dos pedidos e fechamentos no chat.

---

## 🖼️ 4. Imagens das Telas da Aplicação
<img width="1898" height="783" alt="Captura de tela 2026-11-04 182329" src="https://github.com/user-attachments/assets/d517c5aa-4cfe-4476-98ae-4939f844abea" />

<img width="1904" height="798" alt="Captura de tela 2026-11-04 182353" src="https://github.com/user-attachments/assets/9bd3acb0-dbbb-4108-903f-69838648610e" />

<img width="1906" height="901" alt="Captura de tela 2026-11-04 182410" src="https://github.com/user-attachments/assets/69df96f8-ffc6-4df7-8b04-48bee8c8caaf" />

## 📋 5. O Mega Prompt e as Correções Posteriores

<details>
<summary><b>Clique para expandir o Mega Prompt inicial usado no Lovable</b></summary>

```markdown
MVP Estruturado
Landing Page (/)
Hero Section

Objetivo: gerar desejo e incentivar a ação.

Elementos:

Monograma/Logo "VC"
Headline:

Exclusividade, Elegância e Caimento Perfeito.

Subheadline:

Peças selecionadas para mulheres que valorizam estilo e autenticidade.

CTA principal: Monte Seu Look
Produtos em Destaque

Card da peça com:

Imagem
Nome
Categoria
Preço
Botão "Reservar"

Exemplo:

Plain Text
Vestido Bordeaux Elegance
Categoria: Vestido
R$ 489,90
 
[ Reservar ]
Formulário "Monte Seu Pedido"

Campos:

Dados da Cliente
Nome
WhatsApp
Tipo de Peça
Vestido
Conjunto
Alfaiataria
Acessório
Tamanho
PP
P
M
G
Estilo
Casual Chic
Noite
Alfaiataria
Observações

Campo livre opcional.

Integração WhatsApp

Ao clicar em:

"Enviar Pedido"

Será gerado automaticamente:

Plain Text
Olá Vinasco Closet!
 
Gostaria de reservar uma peça.
 
Nome: Ana Paula
Tipo: Vestido
Tamanho: M
Estilo: Noite
 
Aguardo atendimento.

Redirecionamento:

Plain Text
https://wa.me/55XXXXXXXXXXX?text={mensagem}
Painel Administrativo (/admin)
Dashboard
KPIs

Cards superiores:

Indicador	DescriçãoTotal Pedidos	Todos os registros
Leads Ativos	Não concluídos
Faturamento Estimado	Soma dos valores
Pedidos Hoje	Novos registros
Gestão de Pedidos

Tabela:

Cliente	Peça	Tamanho	Estilo	StatusAna	Vestido	M	Noite	Novo Pedido
Status

Fluxo:

Plain Text
Novo Pedido
↓
Em Separação
↓
Concluído

Cores:

Novo → Dourado
Em Separação → Bordô
Concluído → Verde
Modelo de Dados (MVP)
Produtos
TypeScript
Product {
id
name
category
price
imageUrl
active
}
Pedidos
TypeScript
Order {
id
customerName
customerPhone
itemType
size
style
notes
status
createdAt
}
Stack Recomendada
Frontend
Next.js
React
TypeScript
Tailwind CSS
shadcn/ui
Banco

MVP:

Supabase

Tabelas:

products
orders
Hospedagem
Vercel
Critérios de Sucesso do MVP

Após o lançamento, medir:

Número de visitantes
Quantidade de formulários enviados
Cliques para WhatsApp
Conversão em venda
Ticket médio estimado
Roadmap Pós-MVP
Fase 2
Login administrativo
Catálogo completo
Upload de fotos
Busca e filtros
Fase 3
Estoque automático
Integração PIX
Checkout online
Histórico de clientes
CRM integrado
