# Backend Developer | Python & FastAPI

Profissional de TI com sólida experiência em suporte e infraestrutura (Debian/Linux), atualmente focando meu desenvolvimento profissional na construção de APIs robustas e escaláveis no backend web com FastAPI.

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

5.  **[Organização e Arquitetura com APIRouter](https://github.com/sidneylcarneiro/exercicio-apirouter)**
    * **Problema:** Arquivos `main.py` gigantes (monolíticos) causando dificuldade de manutenção e documentação confusa.
    * **Solução:** Refatoração da arquitetura dividindo rotas por domínios de negócio utilizando o `APIRouter`.
    * **Garantia:** Separação de responsabilidades (SoC) e organização visual automática via tags no Swagger UI.

6.  **[Injeção de Dependências e Conexões Seguras](https://github.com/sidneylcarneiro/exercicio-injecao-dependencia)**
    * **Problema:** Conexões de banco de dados presas (memory leaks) devido a exceções e erros não tratados nas rotas.
    * **Solução:** Uso do sistema de `Depends` do FastAPI e funções geradoras (`yield` e `finally`) para garantir o fechamento de conexões de forma automática.
    * **Garantia:** Logs de terminal comprovando o encerramento do banco de dados mesmo após requisições com código 404.

7.  **[Performance com Tarefas em Segundo Plano](https://github.com/sidneylcarneiro/exercicio-background-tasks)**
    * **Problema:** Gargalos de processamento síncrono (ex: envio de e-mails), travando a resposta da API e causando telas de carregamento infinito para o usuário.
    * **Solução:** Implementação do `BackgroundTasks` para delegar tarefas pesadas para os bastidores.
    * **Garantia:** Redução do tempo de resposta da API de 5 segundos para milissegundos, comprovado via logs de execução.

---

## 📫 Perfil
* **GitHub:** [sidneylcarneiro](https://github.com/sidneylcarneiro)
* **Linkedin:** [sidneylcarneiro](https://linkedin.com/in/sidneylcarneiro)
