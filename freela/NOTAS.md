# Saborite Freela - Landing Page

**URL:** https://saborite.com.br/freela/  
**App:** https://freela.saborite.com.br/  
**Criado:** 08/02/2026

---

## 📋 Informações Atuais

### Planos (3 opções com toggle Mensal/Anual)

**SOLO - Pequeno Comércio**
- Mensal: R$ 29/mês
- Anual: R$ 299/ano (R$ 24,92/mês - economiza 14%)
- 1 usuário
- Todos os recursos básicos

**EQUIPE - Gestão em Equipe** (⭐ RECOMENDADO)
- Mensal: R$ 69/mês
- Anual: R$ 699/ano (R$ 58,25/mês - economiza 14%)
- Até 3 usuários simultâneos
- Permissões por usuário
- Dashboard gerencial

**EMPRESARIAL - Múltiplas Lojas**
- Mensal: R$ 149/mês
- Anual: R$ 1.499/ano (R$ 124,92/mês - economiza 14%)
- Usuários ilimitados
- Multi-tenant (múltiplas lojas/filiais)
- API para integrações
- Gerente de conta dedicado

**Addon IA WhatsApp (preço escalonado por plano):**
- Solo: +R$ 9,90/mês
- Equipe: +R$ 19,90/mês
- Empresarial: +R$ 29,90/mês
*(valor varia conforme volume de chamadas API e número de usuários)*

### Funcionalidades Destacadas
✅ Gestão ilimitada de pedidos  
✅ Cadastro ilimitado de clientes  
✅ Controle financeiro completo  
✅ Relatórios e dashboards  
✅ Acesso mobile e desktop  
✅ Suporte (e-mail no mensal, prioritário no anual)

### 🛫 Sistema de Standby (Sobreaviso) e Fila de Espera
**Como na aviação:** Seu negócio não pode parar!

**Standby (Sobreaviso):**
- Freelancer fica em casa, à disposição para assumir em até 1 hora
- Percentual configurável: geralmente 10-30% da diária
- Exemplo: Diária R$ 150 → Standby R$ 15 a R$ 45

**Fila de Espera:**
- Freelancers de backup
- Percentual menor: geralmente 2% da diária
- Exemplo: Diária R$ 150 → Fila R$ 3

**Sistema Automatizado:**
- ⚙️ Freelancer faltou? Sistema convoca standby automaticamente
- ⚙️ Standby acionado? Sistema promove fila de espera para standby
- ⚙️ Calcula tudo: diárias, sobreaviso, fila de espera
- ⚙️ **Registra diferença da diária** para pagamento quando aprovado
- ⚙️ Zero trabalho manual, zero erro de cálculo

**🔒 Segurança Financeira:**
- **TODOS os pagamentos requerem aprovação do financeiro**
- Sistema apenas calcula e registra valores
- Você mantém controle total sobre quando e quanto pagar
- Integração PIX disponível após aprovação
- Nenhum pagamento ocorre automaticamente sem autorização

### 🤖 Addon: Assistente IA via WhatsApp (Preço Escalonado)
**Novidade:** Controle TODO o sistema pelo WhatsApp usando IA!

**Preços por plano:**
- **Solo:** +R$ 9,90/mês
- **Equipe:** +R$ 19,90/mês  
- **Empresarial:** +R$ 29,90/mês

*(Valor escalonado conforme volume de chamadas API e número de usuários)*

**Exemplos de comandos:**
- "Preciso de 2 garçons para sábado" → Cria evento + envia convites
- "Quem está confirmado para hoje?" → Lista completa
- "Quanto gastei com freelancers esse mês?" → Relatório instantâneo
- "Pague João da Silva" → PIX processado
- "Me manda o relatório para o contador" → PDF gerado

**Vantagens:**
- Linguagem natural (fale como se fosse com um colaborador)
- Disponível 24/7
- Integração total com o sistema
- Sem precisar fazer login ou abrir app

---

## 🚀 Próximas Melhorias

### 1️⃣ **Integração Automática de Pagamento (Asaas)**

Atualmente: WhatsApp manual  
**Ideal:** Checkout automático na página

**Como implementar:**
```bash
# Criar cobranças via Asaas API
asaas payments create \
  --customer ID_CLIENTE \
  --value 29.00 \
  --dueDate 2026-03-08 \
  --description "Saborite Freela - Plano Mensal"

# Retorna link de pagamento:
# https://www.asaas.com/c/xyz123
```

**Botão "Assinar Agora" → Redireciona para:**
- Formulário de cadastro (nome, email, CPF)
- Cria cliente no Asaas automaticamente
- Gera cobrança recorrente
- Redireciona para página de pagamento
- Webhook notifica quando pago → cria conta no app

### 2️⃣ **Depoimentos de Clientes**

Adicionar seção de avaliações/depoimentos:
- Fotos de clientes (com permissão)
- Nome + profissão (ex: "Maria Silva, Chef de Eventos")
- Avaliação em estrelas + texto

### 3️⃣ **Vídeo Demo**

Criar vídeo curto (1-2min) mostrando:
- Login no sistema
- Cadastrar um pedido
- Ver dashboard financeiro
- Mobile responsivo

Embed YouTube no hero ou seção dedicada.

### 4️⃣ **Comparativo de Planos (Tabela)**

Tabela lado a lado mostrando o que cada plano inclui:
| Recurso | Mensal | Anual |
|---------|--------|-------|
| Pedidos ilimitados | ✅ | ✅ |
| Clientes ilimitados | ✅ | ✅ |
| Relatórios | ✅ | ✅ |
| Suporte prioritário | ❌ | ✅ |
| Preço/mês | R$ 29 | R$ 24,92 |

### 5️⃣ **Trial Gratuito (Opcional)**

Considerar 7 dias grátis para novos usuários:
- Não precisa cartão
- Webhook cria conta temporária
- Depois de 7 dias, pede assinatura

### 6️⃣ **SEO & Analytics**

✅ Meta tags OK  
✅ Schema.org: Adicionar structured data de produto/SaaS  
⏳ Google Analytics: Instalar tracking  
⏳ Google Tag Manager: Eventos de conversão (clique "Assinar")  
⏳ Facebook Pixel: Remarketing

### 7️⃣ **Chat de Suporte**

Integrar chat ao vivo:
- WhatsApp Business API (via Evolution)
- Ou widget de chat (Tawk.to, Crisp)

---

## 🔧 Manutenção

**Atualizar preços:**
```bash
nano /tmp/sites-placeholder/saborite.com.br/freela/index.html
# Buscar "R$29" e "R$299"
docker restart saborite-com-br
```

**Alterar WhatsApp:**
```bash
# Buscar por: wa.me/5527981125528
# Trocar por novo número
```

**Adicionar nova FAQ:**
```html
<div class="faq-item">
    <div class="faq-question">
        <span>Sua pergunta aqui?</span>
        <span class="faq-toggle">+</span>
    </div>
    <div class="faq-answer">
        <p>Resposta aqui.</p>
    </div>
</div>
```

---

## 📊 Métricas para Acompanhar

- **Visitas à página** (Google Analytics)
- **Taxa de conversão** (cliques "Assinar" / visitas)
- **Plano mais escolhido** (Mensal vs Anual)
- **Origem do tráfego** (Google, redes sociais, direto)
- **Bounce rate** (% que sai sem interagir)

---

## 🎨 Design

**Cores:**
- Primária: #FF6B35 (laranja vibrante)
- Secundária: #F7931E (amarelo-laranja)
- Gradiente: 135deg do laranja para amarelo
- CTA: Mesmo gradiente + sombra

**Fontes:**
- System fonts (rápido carregamento)
- Sans-serif moderno

**Mobile:**
- 100% responsivo
- Cards empilham em mobile
- Botões touch-friendly (mínimo 44x44px)

---

**Desenvolvido por:** Agência do Sucesso Empresarial  
**Contato:** mauricio@sucesso.com.br
