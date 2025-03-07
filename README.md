# resumo-do-lab
Este é um repositório contendo o resumo das lições aprendidas durante o desenvolvimento do lab na DIO".

SLA-->(Service Level Agreement)
Uma SLA de 99% aceita um tempo de inatividade de 1,7 horas
aprox por semana.
Quando maior a quantidade de 9s maior a precisão, a demanda 
do servidor, menor tempo indisponivel.
para se criar uma maquina virtual no Portal Microsoft
é necessario definir: 
- A regiao da maquina virtual
- As opcões de disponibilidade
- Tipo de segurança
- As zonas de disponibilidade
  
## Criação de uma Máquina Virtual

Ao prosseguir com a criação de uma máquina virtual, é fundamental considerar alguns pontos importantes para garantir o correto funcionamento e a otimização dos recursos. Primeiramente, deve-se escolher o tipo de imagem a ser utilizada, como Windows ou Linux, dependendo das necessidades do sistema e do software a ser executado. Além disso, é crucial definir as configurações de rede, incluindo acesso à internet, tipo de conexão e requisitos de monitoramento para garantir a segurança e a eficiência da comunicação entre a máquina virtual e outros sistemas.

Outro aspecto que exige atenção especial é o dimensionamento adequado dos recursos, como CPU, memória e armazenamento, de acordo com a demanda de utilização. Também é importante configurar corretamente as opções de backup e alta disponibilidade, se aplicável, para garantir a continuidade dos serviços em caso de falhas.

## Testando um Banco de Dados SQL

Ao configurar e testar um banco de dados SQL na nuvem, é necessário seguir alguns passos fundamentais. Primeiramente, é preciso ter uma assinatura ativa no serviço de nuvem escolhido. Em seguida, deve-se definir o nome do banco de dados e escolher ou criar um servidor para hospedá-lo. A localização geográfica do servidor também é importante, pois influencia a latência e a conformidade com as normas de proteção de dados.

Outro ponto essencial é configurar o método de autenticação para o banco de dados, garantindo a segurança no acesso. Além disso, é recomendado definir um modelo de redundância para assegurar a disponibilidade e a recuperação de dados em caso de falhas. Por fim, a ferramenta de cálculo do portal da nuvem geralmente exibirá uma estimativa detalhada do custo mensal associado ao uso desses recursos, permitindo um planejamento financeiro adequado.

## Tipos de Serviço de Nuvem

1. IaaS (Infrastructure as a Service) – Infraestrutura como Serviço
Fornece recursos de computação sob demanda, como máquinas virtuais, redes e armazenamento. Ideal para usuários que precisam de controle sobre o ambiente, mas sem gerenciar hardware físico.

Exemplos no Azure:

- Azure Virtual Machines (Máquinas Virtuais)
- Azure Virtual Network (Rede Virtual)
- Azure Storage (Armazenamento)

2. PaaS (Platform as a Service) – Plataforma como Serviço
Oferece um ambiente de desenvolvimento pronto para uso, permitindo foco no código sem necessidade de gerenciar a infraestrutura subjacente.

Exemplos no Azure:

- Azure App Service (Hospedagem de aplicativos web)
- Azure Functions (Execução de código serverless)
- Azure SQL Database (Banco de dados gerenciado)

3. SaaS (Software as a Service) – Software como Serviço
Fornece aplicações completas baseadas na nuvem, acessíveis pela internet, sem necessidade de instalação ou manutenção.

Exemplos no Azure:

- Microsoft 365 (Pacote de produtividade online)
- Azure DevOps (Ferramentas para desenvolvimento e CI/CD)
- Power BI (Análise de dados e visualizações)

4. FaaS (Function as a Service) – Função como Serviço
Modelo de computação serverless que executa funções sob demanda, cobrando apenas pelo tempo de execução.
Exemplo no Azure:

- Azure Functions
Azure também oferece serviços avançados como AI/ML (Inteligência Artificial e Machine Learning), IoT (Internet das Coisas) e Segurança na Nuvem.

## Configurando Recursos e Dimensionamento em Máquinas Virtuais na Azure
Ao criar uma Máquina Virtual (VM) na Azure, é essencial configurar corretamente os recursos para otimizar desempenho e custos.

1. Escolha do Tipo de VM
A Azure oferece diferentes séries de VMs, cada uma otimizada para casos específicos:
- B-series – Econômicas para cargas de trabalho leves.
- D-series – Uso geral, bom equilíbrio entre CPU, memória e armazenamento.
- E-series – Otimizada para cargas intensivas de memória.
- F-series – Alta performance de CPU, ideal para computação intensiva.
- N-series – Com GPUs para workloads de IA e gráficos avançados.

2. Configuração de Recursos
- CPU e Memória: Definidos pelo tamanho da VM escolhida.
- Armazenamento: Uso do Azure Managed Disks (HDD, SSD Standard ou SSD Premium).
- Rede: Configuração de IP público, VNET e regras de segurança (NSG).

3. Dimensionamento (Scaling)
A Azure permite ajustar os recursos conforme a demanda:
- ✅ Scale Up (Vertical) – Aumenta o tamanho da VM (mais CPU/RAM).
- ✅ Scale Out (Horizontal) – Adiciona mais instâncias da VM (usando Azure Virtual Machine Scale Sets).

4. Otimização de Custos
- 💰 Reserved Instances (RI) – Planos de 1 ou 3 anos com desconto.
- 💰 Spot VMs – Custo reduzido para workloads não críticos.
- 💰 Auto Scaling – Ajusta automaticamente o número de VMs conforme a carga.
