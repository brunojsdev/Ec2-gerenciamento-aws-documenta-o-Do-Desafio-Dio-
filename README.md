# Gerenciamento de Instâncias EC2 na AWS

## 📌 Descrição do Desafio

Este repositório documenta a execução de um laboratório conceitual sobre **gerenciamento de instâncias EC2 na AWS**, desenvolvido como parte de um desafio da DIO.

O objetivo é consolidar os conhecimentos adquiridos nas aulas por meio de **documentação técnica estruturada**, simulando um ambiente real de nuvem, com nomes, regiões e configurações utilizadas no mercado.

Todo o conteúdo foi produzido utilizando **Visual Studio Code** e **GitHub**, sem a criação de recursos pagos na AWS, respeitando o caráter educacional do desafio.

---

## 🎯 Objetivos de Aprendizagem

* Compreender o funcionamento do Amazon EC2
* Planejar a criação e o gerenciamento de instâncias
* Aplicar boas práticas de segurança, monitoramento e custos
* Documentar processos técnicos de forma clara e profissional
* Utilizar o GitHub como ferramenta de versionamento e estudo

---

## 🌎 Contexto do Ambiente Planejado

As configurações abaixo representam um cenário **realista e amplamente utilizado em ambientes profissionais**.

* **Região AWS:** sa-east-1 (São Paulo)
* **Finalidade:** laboratório de estudo e desenvolvimento
* **Modelo de cobrança:** On-Demand (Free Tier quando aplicável)

---

## 🖥️ Detalhes da Instância EC2

### Identificação

* **Nome da instância:** ec2-web-server-lab
* **Sistema operacional (AMI):** Amazon Linux 2 (x86_64)
* **Tipo de instância:** t2.micro

### Justificativa

A instância t2.micro foi escolhida por ser elegível ao Free Tier e adequada para ambientes de aprendizado, enquanto o Amazon Linux 2 é otimizado para serviços AWS e amplamente utilizado em produção.

---

## 🔐 Segurança

### Security Group

* **Nome:** sg-web-ec2-lab

**Regras configuradas:**

* Porta 22 (SSH): acesso restrito ao IP do administrador
* Porta 80 (HTTP): acesso liberado para a internet (0.0.0.0/0)

### IAM Role

Foi planejada a associação de uma IAM Role com permissões controladas para acesso a outros serviços AWS, evitando o uso de credenciais estáticas dentro da instância.

---

## 💽 Armazenamento

* **Tipo de volume:** Amazon EBS gp3
* **Tamanho:** 8 GB
* **Nome do volume:** ebs-root-ec2-lab

O volume EBS garante persistência dos dados mesmo após reinicializações da instância.

---

## 📊 Monitoramento

O monitoramento da instância foi planejado utilizando o **Amazon CloudWatch**.

### Métricas acompanhadas

* CPUUtilization
* NetworkIn
* NetworkOut

### Alarmes

* Alerta configurado para notificar quando a utilização de CPU ultrapassar 80%

---

## 💰 Gestão de Custos

Medidas adotadas para controle de custos:

* Utilização de instância t2.micro
* Uso consciente do modelo On-Demand
* Planejamento para desligamento da instância quando não estiver em uso
* Acompanhamento de gastos via AWS Cost Explorer

Essas práticas ajudam a evitar cobranças desnecessárias em ambientes de estudo.

---

## 📂 Estrutura do Repositório

```
ec2-gerenciamento-aws/
├── README.md
├── notes/
│   ├── ec2-conceitos.md
│   ├── ec2-criacao.md
│   ├── ec2-seguranca.md
│   ├── ec2-monitoramento.md
│   └── ec2-custos.md
└── images/
```

---

## 🛠️ Ferramentas Utilizadas

* Visual Studio Code
* Git
* GitHub
* Documentação Oficial da AWS

---

## 📚 Referências

* Documentação oficial da AWS – Amazon EC2
* Materiais da plataforma DIO
* GitHub Markdown Guide

---

## ✅ Conclusão

Este desafio permitiu consolidar conceitos essenciais sobre o gerenciamento de instâncias EC2, reforçando a importância da documentação técnica, organização de recursos e boas práticas em ambientes de computação em nuvem.


---

## 👤 Autor
**brunojsdev**  
