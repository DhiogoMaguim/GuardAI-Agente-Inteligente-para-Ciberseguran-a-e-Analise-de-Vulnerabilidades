# 🛡️ GuardAI — Agente Inteligente para Cibersegurança e Análise de Vulnerabilidades

O **GuardAI** é um agente inteligente focado em **Application Security (AppSec)**, projetado para analisar códigos-fonte, identificar falhas de segurança comuns e propor correções práticas com base em boas práticas de desenvolvimento seguro.

## ✨ Funcionalidades

- **Análise Automatizada de Vulnerabilidades:** Inspeciona trechos de código em busca de brechas de segurança utilizando skills especializadas (`vulnerability-analysis`).
- **Base de Conhecimento em AppSec:** Consulta diretrizes fundamentais de segurança (`security-basics.md`) para embasar os diagnósticos.
- **Sugestão de Correção (Before & After):** Demonstra na prática como transformar um código vulnerável (`app.py`) em uma versão segura (`app_fixed.py`).
- **Validação com Testes:** Inclui rotinas de teste (`test_login.py`) para validar o comportamento seguro da aplicação[cite: 2].

## 🗂️ Estrutura do Projeto

```text
dio-agent-appsec/
├── agent/
│   └── knowledge/
│       └── security-basics.md       # Base de conhecimento com conceitos essenciais de segurança[cite: 2]
├── docs/
│   └── APPSEC-ADDITIONS.md          # Documentação complementar de AppSec[cite: 2]
├── examples/
│   ├── app.py                       # Exemplo de aplicação com vulnerabilidade[cite: 2]
│   └── app_fixed.py                 # Versão corrigida e segura da aplicação[cite: 2]
├── skills/
│   └── vulnerability-analysis/
│       └── SKILL.md                 # Instruções e regras da skill de análise de vulnerabilidades[cite: 2]
├── tests/
│   └── test_login.py                # Testes automatizados de autenticação[cite: 2]
└── integrate.py                     # Script principal de integração do agente[cite: 2]
