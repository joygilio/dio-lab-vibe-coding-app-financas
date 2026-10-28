# 📊 FinaApp - Sistema de Gestão Financeira Pessoal

O **FinaApp** é uma plataforma moderna de controle financeiro desenvolvida como projeto de conclusão de curso. O ecossistema foi projetado com foco total em **Experiência do Usuário (UX)**, privacidade de dados e interfaces fluidas, permitindo que os usuários gerenciem suas receitas e despesas com simplicidade e segurança.

---

## 🎯 Diferenciais de UX & Funcionalidades

### 🔐 Autenticação Segura & Recuperação de Fluxo Contínuo
*   **Split-Screen Design:** Tela de login responsiva com divisão de espaço harmônica.
*   **Recuperação Dinâmica:** O fluxo de redefinição de senha (`forgot_password`) alterna os cards na tela sem necessidade de recarregamento (SPA), utilizando `supabase.auth.resetPasswordForEmail`.
*   **Visualização de Senha:** Inputs de senha equipados com botões de alternância visual (`Eye/EyeOff`) para mitigar erros de digitação.

### 👁️ Modo de Privacidade Global (Privacy by Design)
*   **Ocultação de Saldos:** Um botão de alternância global permite ocultar ou exibir todos os valores financeiros, saldos e gráficos da tela com um único clique, protegendo os dados do usuário em ambientes públicos.

### 📈 Dashboard Interativo (Painel)
*   **Visão Geral Instantânea:** Cards de resumo para Entradas (Verde), Saídas (Vermelho) e Balanço Mensal.
*   **Gráficos de Rosca (Recharts):** Distribuição percentual de despesas categorizadas em tempo real.
*   **Histórico Editável:** Listagem das últimas 10 transações onde o clique em qualquer linha abre o fluxo interativo de edição ou exclusão do registro.
*   **Skeletons de Carregamento:** Substituição visual por blocos cinzas animados durante as requisições ao banco de dados, evitando saltos de layout (*Cumulative Layout Shift - CLS*).

---

## 🛠️ Stack Tecnológica

*   **Frontend:** React.js (TypeScript) + Vite
*   **Estilização:** Tailwind CSS
*   **Componentes de UI:** shadcn/ui + Lucide Icons
*   **Gráficos:** Recharts
*   **Backend as a Service (BaaS):** Supabase (PostgreSQL / Auth)

---
Desenvolvido com 💜 LOVABLE e GEMINI focado em Engenharia de Software e Design de Interface.

<img width="3286" height="1080" alt="image" src="https://github.com/user-attachments/assets/b11f8d4d-76b5-4a17-8977-c5273f7e1de9" />

---

## 🤖 Processo de Desenvolvimento & Engenharia de Prompts

Este projeto foi desenvolvido utilizando uma abordagem moderna de **Full-Stack AI Co-Creation**, utilizando o **Lovable** como motor de geração de código (React + Vite + Supabase). 

A engenharia de software foi conduzida através de ciclos iterativos de prompts estruturados, permitindo focar os esforços no design de interação e na experiência do usuário (UX).

### 📝 Resumo dos Prompts Utilizados

O desenvolvimento foi guiado por três blocos principais de instruções:

1.  **Fundação e Fluxo de Autenticação Segura:** Engenharia de prompt focada na criação do sistema de login/cadastro (*split-screen*) e na estruturação lógica do fluxo dinâmico de redefinição de senha (`forgot_password`) integrado ao `supabase.auth.resetPasswordForEmail`.
2.  **Otimização de Componentes e Microinterações:** Instruções para inclusão de controle de visibilidade de inputs de senha (ícones `Eye/EyeOff`) e na replicação dessa lógica para ocultação global de saldos financeiros (Princípio de *Privacy by Design*).
3.  **Dashboard Financeiro e Persistência:** Prompts direcionados para a renderização do painel principal (gráficos do Recharts, tabelas iterativas de transações e modais de inserção de dados), além da automação do mapeamento de tabelas (`profiles` e `transactions`) diretamente no Supabase.

---

## 🗺️ Roadmap de Evolução (Próximos Passos)

- [ ] **Módulo de Perfil:** Upload de foto real utilizando o *Supabase Storage* com validação de formato e tamanho.
- [ ] **Filtros Avançados:** Busca de transações por período (mês/ano) e palavras-chave.
---

## 🧠 Reflexão

### O que funcionou bem?
O refinamento com o Gemini ajudou muito, pois os créditos do Lovable acabam com poucas interações. Essa estratégia de cocriação permitiu manter o ritmo de desenvolvimento mesmo com as limitações da plataforma principal.

### O que não funcionou como o esperado?
O tempo médio para concluir o projeto. Esperava poder interagir mais vezes gratuitamente com o Lovable para finalizar todas as features visadas de primeira.

### O que aprendeu sobre conversar com IAs?
Que quanto mais detalhes conseguimos dar, melhor é o resultado. Para obter sucesso, precisamos ter um bom conhecimento técnico prévio do que estamos fazendo, até porque precisamos guiar a IA, corrigir os erros ou solucionar os eventuais problemas de arquitetura que surgem no caminho.
