# Controle de Finanças

App Android de controle financeiro pessoal.

- Receitas e gastos, separados em fixos e variáveis
- Fixos mensais (aluguel, contas, salário, aporte) com confirmação mês a mês
- Investimentos: aportes e resgates por carteira
- Empréstimos a receber, com vencimento e alerta de atraso
- Metas de gasto por categoria e histórico de 6 meses
- Backup/importação em CSV

## Build

Todo push na `main` dispara o workflow `Build APK`, que gera `financas.apk` e publica em **Releases**.

Para instalar: baixe o `financas.apk` da última release pelo celular e permita instalação de fontes desconhecidas.

Os dados ficam salvos no próprio aparelho. Use **Backup / exportar** periodicamente.

## Estrutura

- `www/index.html` — o app (HTML/CSS/JS, sem dependências)
- `capacitor.config.json` — empacotamento Android via Capacitor
- `.github/workflows/build-apk.yml` — build do APK
