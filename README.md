# 📌 **Modelo EER - Oficina Mecânica**  

Este projeto apresenta um modelo **EER (Enhanced Entity-Relationship)** para o gerenciamento de oficinas mecânicas. O objetivo é estruturar de forma eficiente os **clientes, veículos, mecânicos, ordens de serviço, serviços e peças** dentro do sistema.  

---

## 🏗️ **Visão Geral do Modelo**  

O diagrama EER foi projetado para garantir **integridade, escalabilidade e facilidade de manutenção**. Ele define as **entidades**, seus **atributos** e os **relacionamentos** entre elas, garantindo uma organização eficiente dos dados.  

### **🔹 Entidades Principais**  

1️⃣ **Cliente** – Registra informações sobre os clientes.  
2️⃣ **Veículo** – Associado a um cliente, armazena dados do veículo.  
3️⃣ **Mecânico** – Profissionais que realizam serviços.  
4️⃣ **Equipe** – Agrupamento de mecânicos para atender ordens de serviço.  
5️⃣ **Ordem de Serviço** – Registro das manutenções realizadas.  
6️⃣ **Serviço** – Tarefas executadas em um veículo (ex.: troca de óleo, alinhamento).  
7️⃣ **Peça** – Itens utilizados nas manutenções (ex.: pneus, filtros, baterias).  

---

## 🔗 **Relacionamentos no Modelo**  

✔ **Cliente x Veículo** – Um cliente pode possuir vários veículos (**1:N**).  
✔ **Veículo x Ordem de Serviço** – Um veículo pode ter várias ordens de serviço (**1:N**).  
✔ **Ordem de Serviço x Equipe** – Cada ordem é atribuída a uma equipe (**N:1**).  
✔ **Equipe x Mecânico** – Uma equipe pode ter vários mecânicos e um mecânico pode estar em várias equipes (**N:M**).  
✔ **Ordem de Serviço x Serviço** – Uma ordem pode conter vários serviços e um serviço pode estar em várias ordens (**N:M**).  
✔ **Ordem de Serviço x Peça** – Uma ordem pode incluir várias peças e uma peça pode ser usada em várias ordens (**N:M**).  

---

![HandsOn-Oficina](https://github.com/user-attachments/assets/546ab886-bd89-4211-832a-00787932e526)


## 📊 **Vantagens da Modelagem**  

✅ **Eliminação de Redundância** – A modelagem evita dados duplicados, garantindo eficiência no armazenamento.  
✅ **Integridade Relacional** – O uso de chaves primárias e estrangeiras assegura consistência nos dados.  
✅ **Facilidade de Expansão** – O modelo permite a inclusão de novas funcionalidades sem comprometer a estrutura atual.  

---

## 📜 **Notas sobre Melhorias e Otimizações**  

🔹 **Uso de Chaves Estrangeiras** – Garante consistência e evita registros órfãos.  
🔹 **Tabelas Intermediárias (N:M)** – Foram criadas para representar os relacionamentos muitos-para-muitos corretamente (Equipe-Mecânicos, Ordem-Serviço, Ordem-Peça).  
🔹 **Tipos de Dados Adequados** – Ajuste nos formatos de data, valores monetários e identificadores para garantir eficiência.  

---

## 📌 **Conclusão**  

Este modelo EER garante um **banco de dados bem estruturado**, permitindo consultas rápidas e seguras para o gerenciamento de oficinas mecânicas.  

📂 **Arquivo de referência**: Consulte o diagrama EER para visualizar a estrutura completa.  

🚀 **Pronto para ser implementado!** 🚀  
