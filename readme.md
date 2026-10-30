# 👓 MyOtica (v1.0) — Sistema de Gestão & PDV Rápido para Óticas

O **MyOtica v1.0** foi desenvolvido sob medida por **Lucas Henrique Leonardo de Jesus** para substituir as antigas fichas físicas de papel por um fluxo digital ágil, 100% offline no computador da ótica, com **auto-instalação em `C:\MyOtica` e atalho na Área de Trabalho na primeira execução**, suporte a **Modo Escuro (Dark Mode)**, **atendimento pelo celular (Android e iPhone via Wi-Fi local)**, **backup automático no Google Drive ou OneDrive** e **verificador integrado de atualizações**.

## ✨ Principais Funcionalidades

### ⚡ 1. PDV de Balcão em 15 Segundos (Venda em 2 Etapas)

* **Etapa 1 (Na frente do cliente):** Anote apenas o **Nome**, **Telefone**, **Lente**, **Armação**, **Valor Total** e **Entrada** para imprimir o recibo na hora.

* **Etapa 2 (Pós-venda):** Preencha com calma os dados técnicos da receita (**Esférico, Cilíndrico, Eixo, DNP, ACO, Adição e Código Lab.**) na aba de pendências sem travar o balcão.

### 📁 2. Fichas Digitais Completas (Pedidos e Pagamentos)

* **Histórico de Pedidos:** Registro completo de todas as Ordens de Serviço (OS) do cliente, receitas anteriores, **Código Lab.**, botão **"🔁 Repetir Grau"** e reimpressão com 1 clique.

* **Controle de Pagamentos:** Registro detalhado de entradas, parcelas no crediário, pagamentos via PIX, dinheiro ou cartão, cálculo automático do saldo restante a pagar e botão dedicado **"🖨️ Imprimir Pagamentos"**.

### ⏳ 3. Controle de Laboratório / Produção & Avisos via WhatsApp

* Filtro rápido de pedidos **Em Produção**, **Aguardando Preencher Grau** e **Prontos na Ótica**, com busca direta por **Código Lab.**, nome do cliente ou número da OS.

* Alertas visuais de entrega para hoje ou pedidos atrasados.

* Botão direto **"📲 Avisar no WhatsApp"** com mensagem personalizada automática assim que o óculos chega do laboratório.

### 🏷️ 4. Tabela de Preços & Simulador de Orçamento no Balcão

* Consulta instantânea de lentes (Visão Simples, Multifocais, Filtro Azul, Policarbonato, Alto Índice) e armações.

* **Simulador Rápido:** Combine qualquer lente + armação + desconto para exibir na tela o valor à vista e o parcelamento em **3x, 6x e 10x** na hora para o cliente.

### 📒 5. Planilha Financeira Completa do Mês

* Consolida automaticamente todas as **Vendas (OS)**, **Entradas em Dinheiro**, **Entradas em Cartão/PIX** e todas as **Saídas/Despesas** do mês (laboratório, fornecedores, aluguel, comissões, retiradas), com opção de impressão direta do fechamento mensal.

### 🖨️ 6. Impressão Sofisticada (A4 2 Vias ou A5 1 Via) & Garantia Configurável

* Compatível com qualquer impressora padrão do mercado em dois formatos executivos:

  * **📄 A4 (2 vias):** Imprime a 1ª Via (Controle da Ótica / Laboratório) e a 2ª Via (Comprovante e Garantia do Cliente) na mesma folha A4 com linha de corte.

  * **📄 A5 (1 via):** Imprime uma única via em meia folha A5 (148 x 210 mm).

* **Termo de Garantia Configurável:** Rodapé com mensagem de agradecimento e cláusula automática de garantia de adaptação cujo prazo (padrão: `3 meses`) pode ser alterado livremente na aba de Configurações.

### ☁️ 7. Backup Automático no Google Drive / OneDrive & Atualizações Online

* **Backup em Tempo Real:** Detecta e vincula a pasta do **Google Drive** ou **OneDrive** instalada no computador, salvando uma cópia quente (*Hot Backup*) a cada venda ou pagamento.

* **Atualizações Disponíveis no Programa:** Painel integrado nas configurações que consulta novas versões publicadas pelo desenvolvedor e baixa a atualização preservando 100% dos dados locais.

## 👨‍💻 Sobre o Desenvolvedor & Tecnologias Utilizadas

O **MyOtica** foi idealizado, projetado e desenvolvido por **Lucas Henrique Leonardo de Jesus**, utilizando:

* **Python 3 & Servidor Multithread WSGI (`ThreadingWSGIServer`):** Processamento local e em rede Wi-Fi de alta velocidade.

* **Banco de Dados SQLite3 em Modo WAL (*Write-Ahead Logging*):** Arquitetura relacional ACID com 12 índices de busca rápida, migração automática de esquema e API de *Online Hot Backup* para sincronização em nuvem.

* **Interface Desktop Nativa (`.EXE`), Auto-Instalador `C:\MyOtica` & PWA Mobile:** Compilação via **PyInstaller** + **PyWebView / App Mode**, auto-instalação silenciosa na primeira abertura com criação de atalho na Área de Trabalho via API `WScript.Shell`, gerador binário nativo de ícones (`.ICO` ARGB 32-bits), HTML5, CSS3 com suporte a Modo Escuro e Manifesto *Progressive Web App* para Android e iOS.

* **Segurança Criptográfica (`SHA-256`) & Diagramação Vetorial `@page`:** Licenciamento comercial vinculado ao hardware de cada máquina e impressão universal A4/A5.

## 💻 Como Instalar e Usar (Versão Cliente)

1. Baixe o executável **`SistemaOtica_Cliente.exe`** na aba de **Releases** deste repositório.

2. Dê dois cliques em **`SistemaOtica_Cliente.exe`**. Na primeira execução, ele criará automaticamente a pasta **`C:\MyOtica`** no Disco Local C: e adicionará o atalho **MyOtica** na sua **Área de Trabalho (Desktop)** e no **Menu Iniciar**.

3. Informe o **Código da Máquina** exibido na tela ao fornecedor para receber a sua **Chave de Ativação (Key)**.

4. Cole a sua Chave de Ativação e clique em **🔓 Ativar Sistema Agora**.

## 📱 Como Usar no Celular (Android e iPhone / iOS)

1. Com o programa aberto no computador da ótica, clique na aba **⚙️ Configurações**.

2. Conecte o celular na **mesma rede Wi-Fi** da ótica e digite no navegador (Chrome ou Safari) o endereço indicado na tela (ex.: `http://192.168.1.15:8080/myotica`).

3. Toque em **"Adicionar à Tela Inicial"** para instalar o atalho do aplicativo direto no celular.

## 📞 Suporte Comercial e Licenciamento

Interessado em adquirir uma licença vitalícia ou mensal para a sua ótica? Entre em contato:

* **Desenvolvedor:** Lucas Henrique Leonardo de Jesus

* **WhatsApp Comercial:** (37) 99953-1535

* **E-mail:** lucashenriqueleonardodejesus@gmail.com