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

Com este guia, você estará apto a configurar máquinas virtuais no Azure de forma eficiente e prática. 🚀
