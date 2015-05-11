# OpenShift Maintenance Page

Durante o deploy de sua aplicação, quando a flag `hot_deploy` não está ativa, seus usuário recebem uma página `503` padrão do servidor Apache.
Este cartucho substitui esta página por outra mais amigável, e permite que você personalize o conteúdo da mesma.

### Incluindo a página de manutenção

Para incluir o cartucho da página de manutenção, execute o comando:

```sh
rhc cartridge add http://reflector-getupcloud.getup.io/github/getupcloud/openshift-cartridge-maintenance-page -a <appname>
```

### Costomization

Você pode mudar a página de manutenção especificando uma URL:

```sh
rhc env set MAINTENANCE_URL=https://raw.githubusercontent.com/getupcloud/openshift-cartridge-maintenance-page/100f7feb058036e8376adae4243d6a94f6271be0/lib/503.html -a <myapp>
```

# Créditos

Cartucho original em [openshift-cartridge-maintenance-page repo on GitHub](https://github.com/mignev/openshift-cartridge-maintenance-page).

#Copyright
Copyright (c) 2014 Marian Ignev. See LICENSE for further details.
