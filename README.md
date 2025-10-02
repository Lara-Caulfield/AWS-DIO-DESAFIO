# AWS Step Functions Lab

Evidências do lab com Step Functions, Lambda e CloudWatch.

## Pastas
- `images/`: prints (Lambda, roles, state machine, CloudWatch, SNS).
- `notes/insights.md`: aprendizados.
- `notes/troubleshooting.md`: erros e como resolvi.

## Como reproduzir
- Step Functions → estado Lambda Invoke chamando a função.
- Permissão na Lambda: `states.amazonaws.com` com Source ARN da state machine.
- Input de teste: `{"msg":"teste curso"}`
- Saída esperada: `{"status":"OK","echo":{"msg":"teste curso"}}`
