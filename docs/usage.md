# 📖 Guia de Uso — Consulta de CEP · Bitrix24

## Pré-requisitos

- Conta Bitrix24 (qualquer plano)
- Servidor para hospedar o `index.html` (pode ser GitHub Pages, Netlify, etc.)
- Campos personalizados criados no CRM (ver tabela no README)

---

## Instalação passo a passo

### 1. Hospedar o aplicativo

Você pode hospedar o `src/index.html` de várias formas:

**Opção A — GitHub Pages (gratuito):**
```bash
# Após criar o repositório, ative GitHub Pages em:
# Settings → Pages → Source: main branch / src folder
```

**Opção B — Netlify (gratuito):**
1. Acesse [netlify.com](https://netlify.com)
2. Arraste a pasta `src/` para o deploy

---

### 2. Registrar o App no Bitrix24

1. Acesse: `Bitrix24 → Configurações → Mercado → Criar App`
2. Tipo: **Aplicativo externo (iFrame)**
3. URL do app: `https://SEU_DOMINIO/index.html`
4. Placement: `CRM_CONTACT_DETAIL_TAB` ou `CRM_CONTACT_DETAIL_TOOLBAR`
5. Permissões necessárias: `crm` (leitura e escrita)

---

### 3. Criar os campos personalizados no CRM

No Bitrix24, acesse **CRM → Contatos → Configurações → Campos personalizados** e crie:

| Nome do campo | Tipo   | ID que aparece no código          |
|---------------|--------|-----------------------------------|
| CEP           | Texto  | `UF_CRM_1772350313579`            |
| Logradouro    | Texto  | `UF_CRM_1772350340846`            |
| Bairro        | Texto  | `UF_CRM_1772350608337`            |
| Cidade        | Texto  | `UF_CRM_1772350625864`            |
| Estado        | Texto  | `UF_CRM_1772350638188`            |
| Número        | Texto  | `UF_CRM_1772350591083`            |
| Complemento   | Texto  | `UF_CRM_1772419053`               |

> ⚠️ Se os IDs dos seus campos forem diferentes, edite o objeto `FIELDS` no `src/index.html`.

---

## Como usar

1. Abra um **Contato** no CRM
2. Acesse a aba/painel do app **"Consulta de CEP"**
3. Digite o CEP no campo e clique em **⊕ Buscar**
4. Os campos de endereço serão preenchidos automaticamente
5. Informe o **número** e **complemento** manualmente (opcional)
6. Clique em **✓ Salvar no Contato**

---

## Suporte

Dúvidas? Fale com a equipe LibeSales:  
📧 contato@libesales.com.br
