# ☁️ Computação e Redes no Azure

Este documento resume os principais serviços de **Computação** e **Rede** disponíveis no Microsoft Azure, com foco em seus usos, benefícios e diferenças. Ideal para quem está construindo arquiteturas na nuvem e precisa entender as possibilidades oferecidas pela plataforma.

---

## 🧠 Serviços de Computação do Azure

### 🖥️ Máquinas Virtuais (VMs)

As Máquinas Virtuais são emulações completas de computadores físicos, oferecendo:

- Infraestrutura como serviço (IaaS)
- Suporte a Windows e Linux
- Ideal para migração de sistemas legados (“lift-and-shift”)
- Controle total sobre o ambiente (SO, memória, disco, rede)

**Alta disponibilidade e escalabilidade:**

- **Conjuntos de Dimensionamento de VMs (VMSS):** escalonamento automático e balanceamento de carga
- **Conjuntos de Disponibilidade:** garantem resiliência contra falhas e manutenções

---

### 💻 Área de Trabalho Virtual do Azure (AVD)

- Virtualização de desktops e aplicativos
- Acesso remoto seguro e centralizado
- Redução de custos com infraestrutura
- Escalável para empresas com múltiplos perfis de usuários

---

### 📦 Serviços de Contêineres

Ambiente leve e isolado para execução de aplicativos. Ideal para microsserviços, CI/CD e aplicações em constante mudança.

- **Azure Container Instances (ACI):** roda contêineres sem precisar configurar VMs
- **Azure Kubernetes Service (AKS):** orquestração completa com Kubernetes
- **Azure App Service:** hospedagem de apps e APIs usando contêineres

---

### ⚙️ Azure Functions

- Computação baseada em eventos (serverless)
- Executa código sob demanda, sem necessidade de infraestrutura permanente
- Escalabilidade automática e modelo de pagamento por uso
- Ótimo para automações, integrações e rotinas pontuais

---

## 🌐 Serviços de Rede do Azure

### 🛠️ Rede Virtual do Azure (VNet)

A base para todas as comunicações internas entre recursos Azure.

- Conecta VMs, bancos de dados, contêineres, etc.
- Segmentação com sub-redes
- Comunicação com internet e redes locais
- **Emparelhamento de rede:** comunicação entre VNets diferentes

---

### 🔐 Gateway de VPN

Conecta redes locais ao Azure com segurança via VPN criptografada.

- **Site-to-Site:** conecta sua rede local à nuvem
- **Point-to-Site:** conecta dispositivos individuais
- **VNet-to-VNet:** conecta duas redes virtuais

---

### ⚡ ExpressRoute

- Conexão privada (sem internet) entre o Azure e sua rede local
- Alta velocidade e menor latência
- Mais seguro e confiável para cargas críticas

---

### 🌍 Azure DNS

- Gerenciamento de domínios DNS com alta performance
- Baseado em infraestrutura global da Microsoft
- Suporte a controle de acesso (RBAC) e logs de auditoria
- Integração com redes privadas e nomes DNS personalizados

---

> ✨ **Dica da Profa:** Ao criar VMs no Azure, escolha os recursos conforme o ambiente:
> - **Desenvolvimento/Teste:** camadas gratuitas ou de baixo custo
> - **Produção:** selecione regiões próximas do usuário final e ative redundância com conjuntos de disponibilidade
> - **Contêineres:** use App Service ou AKS para aplicações modernas, escaláveis e leves

---

