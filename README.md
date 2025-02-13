# Guia: Como Criar uma Máquina Virtual no Azure 🌐💻

Este guia fornece um passo a passo detalhado para criar uma máquina virtual no Azure, abordando os principais tópicos, desde a configuração inicial até a conexão à máquina. Ideal para iniciantes e profissionais que desejam configurar um ambiente de nuvem rapidamente.

---

## Passo 1: **Acessar o Portal do Azure**
1. Acesse [Azure Portal](https://portal.azure.com) e faça login com sua conta.
2. Caso não tenha uma conta, crie uma gratuitamente (Azure oferece um crédito inicial para novos usuários).

---

## Passo 2: **Navegar até "Máquinas Virtuais"**
1. No menu lateral esquerdo, clique em **"Máquinas Virtuais"**.
2. Clique em **"Adicionar" > "Criar" > "Máquina Virtual"**.

---

## Passo 3: **Configurar os Detalhes Básicos**
1. **Assinatura**: Selecione a assinatura ativa.
2. **Grupo de Recursos**: Crie um novo grupo ou selecione um existente.
3. **Nome da Máquina Virtual**: Insira um nome único.
4. **Região**: Escolha a localização geográfica para o recurso.
5. **Opção de Disponibilidade**:
   - **Zona de Disponibilidade**: Garante alta disponibilidade.
   - **Conjunto de Escala**: Para balanceamento de carga e escalabilidade.

---

## Passo 4: **Escolher Imagem e Tipo de Tamanho**
1. **Imagem**: Escolha o sistema operacional (Windows, Linux, etc.).
2. **Tamanho**: Selecione o tamanho da VM com base em CPU, memória e custos.

---

## Passo 5: **Configurar Credenciais de Login**
1. Escolha o tipo de autenticação:
   - **Usuário/Senha**: Insira um nome de usuário e senha fortes.
   - **Chave SSH**: Para sistemas Linux, faça o upload ou gere uma chave SSH.
2. Salve as credenciais em local seguro.

---

## Passo 6: **Configurar Disco de Armazenamento**
1. **Tipo de Disco**:
   - SSD Premium (alta performance).
   - SSD Padrão ou HDD (custo-benefício).
2. **Tamanho do Disco**: Ajuste de acordo com sua necessidade.
3. Configure discos adicionais se necessário.

---

## Passo 7: **Configurar Rede**
1. **Rede Virtual**: Use uma rede existente ou crie uma nova.
2. **Sub-rede**: Escolha ou crie uma sub-rede.
3. **Endereço IP Público**: Configure um IP estático ou dinâmico.
4. **Grupo de Segurança de Rede (NSG)**:
   - Configure regras de entrada/saída para portas específicas, como **RDP (porta 3389)** para Windows ou **SSH (porta 22)** para Linux.

---

## Passo 8: **Configurações Avançadas (Opcional)**
1. **Extensões**: Adicione scripts ou softwares adicionais durante a criação.
2. **Monitoramento**:
   - Habilite diagnósticos de inicialização.
   - Configure métricas e logs para monitoramento.

---

## Passo 9: **Revisar e Criar**
1. Revise todas as configurações.
2. Clique em **"Criar"** para iniciar a implantação.
3. Aguarde a criação da VM (pode levar alguns minutos).

---

## Passo 10: **Conectar à Máquina Virtual**
1. **Windows**:
   - Faça o download do arquivo RDP pelo portal.
   - Conecte-se usando as credenciais configuradas.
2. **Linux**:
   - Use o terminal ou ferramenta SSH para conectar:
     ```bash
     ssh usuario@<endereço-ip>
     ```

---

## Dicas Finais:
- **Custos**: Acompanhe os custos da VM no portal para evitar surpresas.
- **Backup**: Configure backups automáticos para proteger seus dados.
- **Escalabilidade**: Considere adicionar conjuntos de escalas ou balanceadores de carga para maior robustez.

---

Resumo do Módulo 3: Gerenciamento e Governança - Gerenciamento de Custos no Microsoft Azure

Este material aborda os principais conceitos de gerenciamento de custos no Microsoft Azure, com foco em como controlar e otimizar os gastos relacionados aos serviços da plataforma.

Roteiro de Aprendizagem:

Gerenciamento de Custos:

Utilização da Calculadora de Custos e Preços

Implementação de estratégias de gerenciamento de custos e marcas.

Objetivos do Módulo:

Identificar os fatores que influenciam os custos no Azure.

Comparar e contrastar a Calculadora de Preços e a Calculadora de Custo Total de Propriedade (TCO).

Compreender o funcionamento da Ferramenta de Gerenciamento de Custos do Azure.

Entender a finalidade e aplicação das marcas (tags) para organização e controle de custos.

Fatores que Afetam os Custos:

Tipo de Recurso: Os custos variam conforme o tipo de recurso utilizado.

Consumo: O modelo de pagamento "pague pelo que usar" torna o consumo um fator crucial nos custos.

Manutenção: Monitorar e otimizar o ambiente Azure pode reduzir custos, como desligar máquinas virtuais subutilizadas.

Área Geográfica: Os preços dos recursos podem variar dependendo da região geográfica.

Tráfego de Rede: A transferência de dados de saída e entre recursos do Azure pode gerar custos, dependendo das zonas de cobrança.

Assinatura: O tipo de assinatura (ex: avaliação gratuita) influencia os custos.

Explorar o Azure Marketplace:

O Azure Marketplace oferece uma variedade de aplicações e serviços de terceiros, certificados para execução no Azure.

Inclui plataformas de contêiner de software livre, imagens de máquinas virtuais e bancos de dados, ferramentas de desenvolvimento e muito mais.

Calculadora de Preços:

Ferramenta para estimar o custo dos produtos do Azure.

Permite configurar opções como região, camada, opções de cobrança e suporte, programas e ofertas, e preço de Desenvolvimento/Teste do Azure.

Calculadora de Custo Total de Propriedade (TCO):

Ferramenta para estimar a economia de custos ao migrar para o Azure.

Compara os custos das infraestruturas locais com os custos do Azure na nuvem.

Gerenciamento de Custos do Azure:

Relatórios: Geração de relatórios de cobrança.

Enriquecimento de dados para análise detalhada.

Orçamentos: Definição de orçamentos de gastos.

Alertas: Notificações quando os custos excedem os limites definidos.

Recomendações: Sugestões para otimizar os custos.

Marcas (Tags):

Metadados adicionados aos recursos do Azure.

Organizam os recursos em uma taxonomia lógica.

Consistem em pares nome-valor.

Úteis para reunir informações de cobrança e facilitar o gerenciamento.
