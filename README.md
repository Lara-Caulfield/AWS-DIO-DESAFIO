# AWS Step Functions Lab

## O que foi feito
- Criação de uma função Lambda
- Criação de uma State Machine** no AWS Step Functions para invocar a Lambda.
- Configuração das permissões (IAM Role e Resource-based policy) para permitir que o Step Functions invoque a Lambda.
- Testes de execução no Step Functions com input e saída esperada.
- Ativação de logs e métricas no CloudWatch.
- Criação de um **SNS topic** para alertas (e-mail).

## Evidências
As imagens das configurações e execuções estão na pasta `images/`:
- Lambda e permissões
- IAM Role
- State Machine
- Execução bem sucedida
- CloudWatch

## Código da Lambda (exemplo)
```python
def lambda_handler(event, context):
    return {
        "status": "OK",
        "echo": event
    }
