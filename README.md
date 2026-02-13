# Landing Page - Produto Low Ticket

## Visão Geral do Projeto

Este projeto consiste em uma **Landing Page de Alta Conversão** desenvolvida para a venda de um produto digital "Low Ticket" (baixo valor). O foco principal é capturar tráfego vindo de anúncios do Facebook (Facebook Ads), especialmente em dispositivos móveis, e converter visitantes em compradores o mais rápido possível.

O design segue princípios minimalistas para evitar distrações, utilizando gatilhos mentais como escassez, prova social e autoridade para maximizar a taxa de conversão.

## Tecnologias Utilizadas

O projeto foi construído utilizando apenas tecnologias web padrão, sem dependência de frameworks ou bibliotecas externas pesadas, garantindo o máximo de performance.

- **HTML5**: Para estruturação semântica e acessível do conteúdo.
- **CSS3**: Para estilização, layout responsivo e animações focadas em conversão.
- **JavaScript (Vanilla)**: Para interações leves, como rolagem suave (smooth scroll).

## Estrutura de Pastas

A organização do projeto é simples e direta, facilitando a manutenção e o upload para servidores de hospedagem estática.

```
/
├── index.html       # Arquivo principal da página (Estrutura)
├── css/
│   └── style.css    # Folha de estilos (Design e Responsividade)
└── js/
    └── script.js    # Scripts de interação (Funcionalidade)
```

### Detalhes dos Arquivos

- **`index.html`**: Contém toda a estrutura da página.
  - **Header (Hero)**: Headline forte, subheadline explicativa e botão CTA (Call to Action) principal com gatilho de escassez.
  - **Section (Benefícios)**: Lista clara do que o usuário ganha ao comprar o produto.
  - **Section (Prova Social)**: Depoimentos de clientes para gerar confiança.
  - **Section (Oferta/Checkout)**: Preço, garantia e formas de pagamento, com um botão final de compra.
  - **Footer**: Links institucionais obrigatórios para anúncios (Termos de Uso, Privacidade).

- **`css/style.css`**: Define a identidade visual.
  - Usa variáveis CSS (`:root`) para facilitar a troca de cores.
  - Implementa um design responsivo utilizando `flexbox` e `grid`.
  - Possui animações (`@keyframes pulse`) para destacar os botões de compra.

- **`js/script.js`**:
  - Adiciona o comportamento de rolagem suave quando o usuário clica nos botões, levando-o diretamente para a seção de checkout de forma fluida.

## Decisões Técnicas

### Por que Código Puro (Vanilla)?

Optamos por não usar frameworks (como Bootstrap, React ou Tailwind) para manter o **peso da página extremamente baixo**. Em campanhas de tráfego pago, cada milissegundo de carregamento conta. Uma página leve carrega instantaneamente no 3G/4G, reduzindo a taxa de rejeição e aumentando o ROI (Retorno sobre Investimento).

### Performance

- **CSS Externo**: Todo o estilo está em um único arquivo minificável.
- **Google Fonts**: Fontes carregadas com `preconnect` para agilizar a renderização do texto.
- **Imagens**: O uso de ícones leves e emojis no lugar de imagens pesadas mantém o carregamento rápido.

### Design e Conversão

- **Cores**: Verde (`#2ECC71`) para os botões de ação (sinal de "siga", positivo) e Vermelho (`#e74c3c`) para preços e escassez (atenção).
- **Tipografia**: Fonte 'Inter' para máxima legibilidade em telas pequenas.
- **CTA Fixo**: Embora não fixo na tela, os botões são grandes e fáceis de clicar (finger-friendly - zona de toque de 44px+).

## Responsividade (Mobile-First)

A prioridade foi o acesso mobile, já que a maioria do tráfego de redes sociais acessa via celular.

- **Media Queries**: Ajustes específicos para telas menores que 480px e 768px.
- **Grid Layout**: A seção de depoimentos se transforma de 3 colunas (desktop) para 1 coluna (mobile) automaticamente.
- **Tamanhos de Fonte**: Títulos e textos são redimensionados para leitura confortável sem zoom.

## Principais Dificuldades e Soluções

### 1. Ajuste de Responsividade Mobile

- **Dificuldade**: Garantir que o botão de compra e a headline coubessem na primeira dobra em celulares pequenos.
- **Solução**: Ajustei o `padding` da seção Hero e reduzi o tamanho da fonte da headline especificamente para `@media (max-width: 480px)`.

### 2. Otimização de Carregamento (LCP)

- **Dificuldade**: Manter o tempo de carregamento (Largest Contentful Paint) abaixo de 2.5s.
- **Solução**: Eliminação de imagens de fundo pesadas na dobra superior, usando apenas cores sólidas e tipografia forte.

### 3. Foco na Conversão

- **Dificuldade**: Evitar que o usuário se distraísse.
- **Solução**: Remoção de menus de navegação complexos. A única ação possível é rolar a página ou clicar no botão de compra.

## Resultado Final

O projeto entregue é uma landing page **100% funcional**, validada e pronta para produção. Basta subir os arquivos para qualquer hospedagem estática (Vercel, Netlify, GitHub Pages, HostGator, etc.) e configurar o link do botão de compra para o seu gateway de pagamento (Hotmart, Kiwify, Eduzz, etc.).

---

_Projeto desenvolvido por IA Antigravity._
