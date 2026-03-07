# Backend Developer | Python & FastAPI

Profissional de TI com sólida experiência em suporte e infraestrutura (Debian/Linux), atualmente em transição de carreira para o desenvolvimento Backend. Focado em criar soluções robustas, escaláveis e bem documentadas.

---

## 🚀 Tecnologias & Ferramentas
* **Linguagens:** Python
* **Frameworks:** FastAPI, Next.js
* **Banco de Dados:** PostgreSQL, SQLAlchemy, SQLite
* **Infraestrutura:** Docker, Debian Linux, Shell Script
* **Testes & Qualidade:** Pytest, Pydantic (Validação de Dados)
* **Segurança:** Autenticação JWT

---

## 📂 Estudos de Casos & Resolução de Problemas
Como parte da minha evolução técnica, estou documentando a resolução de 10 problemas críticos de backend que impactam a performance e segurança de aplicações reais.

1.  **[Validação de Dados com FastAPI & Pydantic](https://github.com/sidneylcarneiro/exercicio-validacao)**
    * **Problema:** Entrada de dados inconsistentes (idades negativas, e-mails inválidos).
    * **Solução:** Implementação de camadas de proteção com Pydantic Fields e tipos especializados.
    * **Garantia:** Cobertura de testes unitários com Pytest.

2.  **[Otimização de Queries - N+1 Problem](https://github.com/sidneylcarneiro/exercicio-n-plus-one)**
    * **Problema:** Lentidão na API devido a múltiplas consultas ao banco de dados dentro de loops (N+1).
    * **Solução:** Implementação de **Eager Loading** com `joinedload` do SQLAlchemy para reduzir 51 consultas para apenas 1.
    * **Garantia:** Monitoramento de logs do Engine SQL para validação de performance.

3.  **[Semântica HTTP e Status Codes](https://github.com/sidneylcarneiro/exercicio-http-semantics)**
    * **Problema:** API retornando `200 OK` para todas as operações, mesmo quando itens não eram encontrados.
    * **Solução:** Implementação de `HTTPException` e códigos de status adequados (`201` para criação, `204` para exclusão e `404` para recursos inexistentes).
    * **Garantia:** Validação visual via Swagger UI e monitoramento de logs de rede.
  
4.  **[Gerenciamento de Variáveis de Ambiente e Segurança](https://github.com/sidneylcarneiro/exercicio-env-variables)**
    * **Problema:** Credenciais sensíveis (URL de banco, tokens de API) fixadas diretamente no código-fonte (hardcoded), expondo a infraestrutura a vazamentos.
    * **Solução:** Implementação do `pydantic-settings` para carregamento de configurações via arquivo `.env`, isolando os segredos da lógica da aplicação.
    * **Garantia:** Configuração estrita do `.gitignore` validada via CLI para impedir o versionamento de dados confidenciais.
---

## 📫 Perfil
* **GitHub:** [sidneylcarneiro](https://github.com/sidneylcarneiro)
* **Linkedin:** [sidneylcarneiro](https://linkedin.com/in/sidneylcarneiro)
