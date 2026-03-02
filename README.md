# 📍 Consulta de CEP — Bitrix24 App

> Aplicativo de preenchimento automático de endereço via CEP para o Bitrix24 CRM.  
> Desenvolvido por **LibeSales** · Parceiros Gold Bitrix24

---

## 🗂️ Estrutura do repositório

```
bitrix24-cep-app/
├── src/
│   └── index.html        # Aplicativo principal (single-file)
├── assets/
│   └── logo.svg          # Logo LibeSales original
├── docs/
│   └── usage.md          # Guia de instalação e uso
└── README.md
```

---

## ✨ Funcionalidades

- 🔍 Consulta de CEP em tempo real via **ViaCEP**
- ✅ Preenchimento automático dos campos de endereço no CRM
- ✏️ Campos manuais para **número** e **complemento**
- 💾 Salvamento direto no registro de **Contato** do Bitrix24
- 🎨 Design **LibeSales** — dark mode, verde #0bbf7e

---

## 🚀 Como instalar no Bitrix24

1. Acesse **Bitrix24 → Mercado de Aplicativos → Adicionar App**
2. Escolha **"Aplicativo por URL"**
3. Informe a URL onde o `src/index.html` está hospedado
4. Configure o placement como **CRM → Contato → Painel lateral**
5. Defina as permissões de acesso ao CRM

---

## 🛠️ Campos CRM mapeados

| Campo    | ID Bitrix24             |
|----------|-------------------------|
| CEP      | `UF_CRM_1772350313579`  |
| Logradouro | `UF_CRM_1772350340846` |
| Bairro   | `UF_CRM_1772350608337`  |
| Cidade   | `UF_CRM_1772350625864`  |
| Estado   | `UF_CRM_1772350638188`  |
| Número   | `UF_CRM_1772350591083`  |
| Complemento | `UF_CRM_1772419053`  |

---

## 🏢 Sobre a LibeSales

**LibeSales** é parceira Gold Bitrix24, especializada em automação de vendas e CRM.

- 🌐 [libesales.com.br](https://libesales.com.br)

---

## 📄 Licença

Uso interno — LibeSales © 2025
