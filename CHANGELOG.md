# 📱 BTP — Histórico de Atualizações

Registro de tudo que foi corrigido e adicionado no app, da atualização mais recente pra mais antiga.

---

## Julho/2026 — Rodada 2 (PRs #9 a #17)

### ✨ Novidades

**Clientes**
- 📤 Exportação de clientes pro WhatsApp: a lista inteira (ou filtrada pela busca) de uma vez, pra qualquer contato ou grupo (#9)
- 📤 Envio de cliente individual pelo WhatsApp com todos os dados cadastrados (#10)
- 📎 Envio do documento anexado do cliente pelo compartilhamento nativo do celular, com fallback de download no computador (#11)

**Vendas**
- 💳 Forma de pagamento na venda: PIX, Dinheiro, Cartão de Crédito, Cartão de Débito, Boleto, Cheque, Transferência (TED), Permuta e Fiado (#12, #13)
- 💵 Entrada opcional em qualquer forma de pagamento + parcelamento de 1x a 12x, com preview ao vivo do valor das parcelas (#13)
- 🧠 Status pago/pendente sugerido automaticamente pela forma de pagamento (#13)
- 🔍 Filtro de vendas (todas / só pendentes / só pagas); tocar no card "A receber" abre direto a lista de cobrança (#14)
- 📊 Todos os painéis de "A receber" passam a contar só o saldo devido, descontando a entrada já paga (#12)

**Orçamentos**
- 🖼️ Card de orçamento repaginado: foto de cada peça, subtotal + frete, prazo de entrega e slogan da marca (#16)
- 🎨 Arte da lona BTP Powertrain como fundo do card, escurecida sem atrapalhar a leitura (#17)
- 📤 Botão "Enviar imagem" abre o compartilhar do celular com o card anexado (#16)

### 🔧 Correções
- Card de orçamento com letras sobrepostas quando havia cliente selecionado (#16)
- Cliente "sumia" do orçamento ao adicionar peças ou editar preço (#16)
- Frete aparecia no texto do orçamento mas não na imagem — os dois saíam com totais diferentes (#16)
- Leitura do CNPJ/CPF no scanner muito melhorada: imagem tratada antes do OCR (ampliação, tons de cinza, contraste) e número validado pelos dígitos verificadores — funciona mesmo com texto bagunçado (#15)
- Cliente sem telefone mostra aviso em vez de abrir link quebrado no WhatsApp (#12)

---

## Julho/2026 — Rodada 1 (PRs #2 a #8)

### ✨ Novidades

**Clientes**
- 📷 Leitura automática de documento (OCR) no cadastro: foto ou PDF de CPF, CNPJ, RG ou CNH preenche nome e documento sozinho (#3, #5)
- 📎 Documento fica anexado ao cadastro, com miniatura e visualização (#3, #5)
- 🏠 Endereço completo com busca automática pelo CEP (ViaCEP) (#3, #5)

**Peças**
- 💧 Marca d'água com a logo BTP carimbada automaticamente nas fotos das peças, sem alterar a logo (#2, #5)
- ✨ Efeito de brilho premium no badge da logo na galeria do catálogo público (#2)
- 🏷️ Etiqueta com QR code por peça pra imprimir e colar no pátio — quem escaneia cai no WhatsApp perguntando por ela (#7)
- 📖 Nova aba **Referência**: banco de peças identificadas (nome correto, código original OEM, modelos que servem, foto), com busca por código ou nome (#8)

**Geral**
- 📲 App instalável no celular (PWA): ícone próprio, tela cheia, funciona offline, sempre busca a versão mais nova quando online (#7)
- ☁️ Atendimentos e Orçamentos passam a sincronizar na nuvem entre os aparelhos, com tolerância a tabela indisponível (#7)
- 📅 Card "Sua semana" no Meu Dia: vendas, comissão e peças da semana com envio no WhatsApp em um toque (#7)
- 🔄 Botão flutuante de atualizar que força buscar a versão mais recente (#6)
- 💬 Follow-up de orçamento parado com mensagem citando a peça e o valor específicos (#7)

### 🔧 Correções
- Texto grudado no menu: "Atendimentos" invadia a aba "Peças" em telas estreitas (#4)
- Atendimentos e Orçamentos eram salvos só no aparelho — cada vendedor via dados diferentes (#7)
- Funcionalidades de OCR/anexo/endereço/marca d'água portadas pro app principal (`index.html`), onde realmente eram usadas (#5)
