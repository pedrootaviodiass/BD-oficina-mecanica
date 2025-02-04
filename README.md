# Sistema de Gerenciamento de Oficina Mecânica 🛠️🚗  

## 🎯 Objetivo do Projeto  
Este sistema foi desenvolvido para **automatizar e otimizar** o gerenciamento de ordens de serviço (OS) em uma oficina mecânica, garantindo:  
- Controle de clientes, veículos e equipes técnicas.  
- Rastreamento do status de cada OS (autorização, execução e conclusão).  
- Cálculo automático de custos (mão de obra + peças).  
- Histórico de serviços para análise futura.  

---

## ⚙️ Funcionalidades Principais  
| Funcionalidade | Descrição |  
|----------------|-----------|  
| **Cadastro de Clientes** | Registro de dados pessoais e veículos associados. |  
| **Gestão de Veículos** | Vinculação de veículos a clientes e histórico de OS. |  
| **Ordens de Serviço (OS)** | Criação de OS com status (`Aguardando`, `Em Andamento`, `Concluída`), datas e valores. |  
| **Autorização do Cliente** | Campo explícito para aprovação antes da execução dos serviços. |  
| **Cálculo de Custos** | Soma automática de serviços e peças com base na tabela de preços. |  
| **Histórico de Preços** | Registro do valor vigente no momento da OS para auditoria. |  

---

## 🔍 Diagrama EER  
![Diagrama Entidade-Relacionamento Estendido](.png)  

### **Entidades e Relacionamentos**  
- **Cliente** ➔ **Veículo** (`1:N`): Um cliente pode ter múltiplos veículos.  
- **Veículo** ➔ **OS** (`1:N`): Cada veículo possui um histórico de ordens de serviço.  
- **OS** ➔ **Equipe** (`1:1`): Uma equipe é responsável por executar a OS.  
- **Equipe** ↔ **Mecânico** (`N:N`): Mecânicos podem atuar em múltiplas equipes.  

*Diagrama criado com [MySql Workbench](https://www.mysql.com/products/workbench/). [Acesse o arquivo editável aqui](docs/diagrama_eer.drawio).*  

---

## 💻 Tecnologias Utilizadas  
- **Banco de Dados:** MySQL  
- **Versionamento:** Git + GitHub  
- **Modelagem:** MySql Workbench
- **Documentação:** Markdown  
