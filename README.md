# Fatec-computacao-nuvem-II-p2

Este repositório contém o arquivo `compose.yml`, que configura e gerencia os serviços do projeto ABA. Ele inclui configurações para o frontend, backend, Grafana e Prometheus.

## Integrantes
 - Witer Xavier Mendonça
 - Daniel França
 - Douglas Hugo


## Pré-requisitos

Certifique-se de que os seguintes softwares estão instalados no seu ambiente antes de usar este arquivo:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

Verifique as versões instaladas com os comandos:

```bash
docker --version
docker-compose --version
```

## Uso

1. **Clone este repositório:**

   ```bash
   git clone https://github.com/witermendonca/Fatec-computacao-nuvem-II-p2.git
   cd Fatec-computacao-nuvem-II-p2
   ```

2. **Inicie os serviços:**

   Execute o comando abaixo para iniciar os contêineres definidos no arquivo `compose.yml`:

   ```bash
   docker-compose up -d
   ```

3. **Verifique os serviços:**

   Liste os contêineres ativos para confirmar se todos os serviços estão em execução:

   ```bash
   docker ps
   ```

4. **Acesse os serviços:**

   - **Frontend:** Acesse em [http://localhost:8081](http://localhost:8081) 

   - **Backend:** Acesse em [http://localhost:8080](http://localhost:8080) 

    - **Backend:Swagger** Acesse em [http://localhost:8080/swagger-ui/index.html#/](http://localhost:8080/swagger-ui/index.html#/)  

   - **Grafana:** Acesse em [http://localhost:3000](http://localhost:3000)  
     Credenciais padrão:
     - Usuário: `admin`
     - Senha: `admin` (altere após o primeiro login)

   - **Prometheus:** Acesse em [http://localhost:9090](http://localhost:9090)  

5. **Parar os serviços:**

   Quando quiser parar os serviços, execute:

   ```bash
   docker-compose down
   ```

## Estrutura do Arquivo `compose.yml`

Os seguintes serviços estão configurados no arquivo:

- **Frontend:**
  - Executa a interface de usuário.
  - Porta: **8081**

- **Backend:**
  - Gerencia a lógica do servidor e APIs.
  - Porta: **8080**

- **Grafana:**
  - Ferramenta de visualização de métricas.
  - Porta: **3000**

- **Prometheus:**
  - Ferramenta de monitoramento e coleta de métricas.
  - Porta: **9090**