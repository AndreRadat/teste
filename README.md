RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS
Data: 18 de março de 2026
Empresa: Abstergo Industries (Divisão de Distribuição Farmacêutica)
Responsável: Dr. André Radatz

Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Dr. Andre Radatz. Atualmente, a empresa opera com infraestrutura de TI on-premise (servidores locais) voltada para a distribuição de medicamentos. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos, eliminar despesas com manutenção de hardware e aumentar a eficiência operacional.

Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: Migração da Infraestrutura de Servidores
Nome da ferramenta: Amazon EC2 (T3 Instances)

Foco da ferramenta: Substituição de servidores físicos por máquinas virtuais na nuvem.

Descrição de caso de uso: Atualmente, a empresa mantém servidores físicos para o sistema de gestão (ERP) e controle de estoque. Com a migração para o EC2, eliminamos custos com eletricidade, refrigeração e manutenção de hardware. Utilizando instâncias da família T3 (burstable), pagamos apenas pelo processamento utilizado, e com o License Manager, garantimos que não haverá custos extras com licenças de sistemas operacionais já adquiridas.

Principal ganho: Fim dos custos de datacenter físico (energia, hardware e refrigeração) e redução de despesas com manutenção de servidores obsoletos.

Etapa 2: Otimização do Armazenamento de Dados e Backups
Nome da ferramenta: Amazon S3 + Backup Automatizado

Foco da ferramenta: Armazenamento seguro e de baixíssimo custo para notas fiscais e registros de lote.

Descrição de caso de uso: A legislação exige que distribuidoras farmacêuticas mantenham registros de rastreabilidade de lotes e notas fiscais por longos períodos. Atualmente, esses dados ocupam espaço caro em servidores de alta performance. Com o Amazon S3 , armazenamos esses dados históricos por um custo aproximadamente 80% menor que soluções tradicionais de fita ou disco, mantendo a acessibilidade quando necessário para auditorias da Anvisa.

Principal ganho: Redução massiva no custo de armazenamento de longo prazo e conformidade regulatória sem gastar fortunas.

Etapa 3: Eliminação de Servidores de Automação e Acesso Remoto
Nome da ferramenta: AWS Lambda + Amazon WorkSpaces

Foco da ferramenta: Computação serverless e substituição de VDI (Virtual Desktop) tradicional.

Descrição de caso de uso:

Lambda: Hoje, a empresa possui servidores rodando apenas para executar tarefas agendadas (como envio de relatórios de vendas e atualização de tabelas de preços). Com o Lambda, essas tarefas viram código executado "sob demanda", sem necessidade de manter uma máquina ligada 24/7.

WorkSpaces: Para a equipe de representantes e conferentes que trabalham remotamente, ao invés de investir em computadores caros ou manter uma estrutura de VPN complexa, utilizamos o WorkSpaces. Eles acessam um desktop virtual leve de qualquer lugar, e o custo é baseado no uso mensal, eliminando a depreciação de equipamentos.

Principal ganho: Redução de custos com licenças de software de acesso remoto (VPN) e eliminação de servidores ociosos que só consumiam energia elétrica.

Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado a redução imediata dos custos com infraestrutura de TI, substituindo despesas fixas por variáveis, eliminando gastos com energia elétrica e manutenção de hardware, e automatizando processos manuais, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa, como soluções de IoT para controle de temperatura de medicamentos durante o transporte.
