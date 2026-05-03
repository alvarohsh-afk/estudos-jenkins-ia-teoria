# Estudos: Jenkins & Infraestrutura como Código (IaC)

Este repositório contém a síntese teórica dos meus estudos sobre automação de infraestrutura e esteiras de implantação (CI/CD). 

## 🚀 Conceitos Fundamentais

### 1. Jenkins e a Esteira CI/CD
O Jenkins atua como o "maestro" da automação. Os principais conceitos teóricos abordados foram:
- **Continuous Integration (CI):** Prática de integrar o código em um repositório compartilhado várias vezes ao dia.
- **Continuous Delivery (CD):** Garantia de que o código esteja sempre pronto para ser implantado.
- **Pipeline:** O fluxo de etapas (Build, Test, Deploy) que o software percorre.

### 2. Infraestrutura como Código (IaC)
A teoria de IaC foca em gerenciar e provisionar infraestrutura através de arquivos de configuração, em vez de processos manuais.
- **Idempotência:** A capacidade de rodar o mesmo script várias vezes e obter sempre o mesmo resultado.
- **Vantagens:** Velocidade, redução de erro humano e facilidade de recuperação em caso de falhas.

## ⚙️ Fluxo de Trabalho (Workflow)
Abaixo, um diagrama do processo teórico de integração:
```mermaid
graph LR
    A[Desenvolvedor] -->|Push Código| B(GitHub)
    B -->|Trigger| C(Jenkins)
    C -->|Executa| D{Scripts IaC}
    D -->|Provisiona| E[Servidor/Nuvem]
