# ARGOS

**Gestão de pecuária e de medicamentos aplicados em bovinos.**

O ARGOS organiza os cadastros da atividade pecuária (propriedades, rebanhos, lotes e animais) para que o produtor tenha um histórico confiável do manejo sanitário. Projeto interdisciplinar do 1º ano do Ensino Médio Técnico em Desenvolvimento de Sistemas.

🌐 [Landing page](https://argos-landingpage.vercel.app/) · 🖥️ [Sistema web](https://argos-web-crud.onrender.com)

## O problema

Na pecuária de corte, o registro das aplicações de medicamentos ainda é feito em papel ou nem é feito. Sem controle, o produtor perde prazos de carência, aplica insumos vencidos e corre o risco de ter lotes retidos ou carne descartada no frigorífico.

## A solução

Um sistema web em que o administrador cadastra e acompanha:

- **propriedades rurais**, com endereço e os usuários responsáveis por cada uma;
- **rebanhos**, **lotes** (engorda, cria e recria) e **animais**, identificados por brinco;
- **usuários** e **administradores**, com login seguro.

Os registros nunca são apagados: a exclusão é lógica, o que preserva o histórico e a rastreabilidade. Os dados alimentam o restante do ecossistema ARGOS, desenvolvido pela equipe do 2º ano (aplicativo, cálculo e alertas de carência).

## ODS 12 — Consumo e produção responsáveis

- **12.2:** manejo responsável dos recursos na pecuária de corte.
- **12.3:** menos perdas e desperdícios por falhas na gestão sanitária.
- **12.4:** controle do uso de medicamentos e vacinas, reduzindo resíduos no ambiente e no alimento.

## Repositórios

| Repositório | Conteúdo |
|---|---|
| [argos-web-crud](https://github.com/projeto-argos/argos-web-crud) | Sistema web em Java (Servlet, JSP e JDBC) |
| [argos-bd](https://github.com/projeto-argos/argos-bd) | Modelos conceitual e lógico, scripts SQL e convenção de nomenclatura |
| [argos-landingpage](https://github.com/projeto-argos/argos-landingpage) | Landing page e telas estáticas do sistema |
| [argos-docs](https://github.com/projeto-argos/argos-docs) | Pesquisas, persona, protótipo e demais artefatos de UX |
| [argos-ai](https://github.com/projeto-argos/argos-ai) | Agente especializado (Gem) e memorial descritivo do uso de IA |

## Tecnologias

| Área | Ferramentas |
|---|---|
| Back-end | Java 21, Jakarta Servlet, JSP, JDBC, HikariCP, Tomcat 11 |
| Banco de dados | PostgreSQL (Aiven) |
| Front-end | HTML, CSS e JavaScript |
| Segurança | BCrypt, Cloudflare Turnstile, variáveis de ambiente |
| Publicação | Render (sistema) e Vercel (landing page) |
| Design e IA | Figma, Canva e Gemini |
| Gestão | Git, GitHub e Jira |

## Equipe

- Eduardo Toledo Alves de Almeida
- Letícia Silva Ribeiro
- Lucca Cansani
- Murilo Gonçalves Paiva
- Pietra de Oliveira Silva Gomes
