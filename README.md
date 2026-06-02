# 📋 Formulário de Negócios · Agendor

Formulário web para registro de novos negócios diretamente no CRM Agendor, sem necessidade de acesso à plataforma.

🔗 **Acesso:** [lucralize-comercial.github.io/formulario-negocios](https://lucralize-comercial.github.io/formulario-negocios/)

---

## Funcionalidades

- Seleção do funil de destino: Legalização, Jurídico ou Regularização
- Busca ou criação automática da organização no Agendor pelo nome da empresa
- Criação do contato (pessoa responsável) vinculado à organização
- Seleção de responsável pelo negócio a partir dos usuários ativos do CRM
- Seleção de produto/serviço a partir do catálogo cadastrado no CRM
- Definição de status (em andamento, ganho ou perdido)
- Data de conclusão obrigatória para negócios ganhos ou perdidos
- Link direto para o negócio criado ao final do envio

## Campos do formulário

| Campo | Destino no Agendor |
|---|---|
| Razão social | Organização (`organizationId`) |
| CNPJ | Campo da organização |
| Pessoa responsável | Pessoa vinculada (`personId`) |
| E-mail | E-mail da pessoa |
| Telefone | Telefone da pessoa |
| Título do negócio | `title` |
| Responsável pelo negócio | `userId` |
| Produto / serviço | `dealProductsAttributes` |
| Valor | `value` |
| Status | `status` |
| Data de início | `startDate` |
| Data de conclusão | `closingDate` |
| Observações | `notes` |

## Configuração

| Item | Valor |
|---|---|
| CRM | Agendor API v3 |
| Funis ativos | Legalização (LGL), Jurídico (JUR), Regularização (REG) |
| Autenticação | Token fixo no arquivo `index.html` |

## Estrutura

```
formulario-negocios/
└── index.html   # Arquivo principal do formulário
```
