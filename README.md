# tolv-magento-2.x

Este módulo foi desenvolvido para que o Tolv funcione corretamente no Magento 2.x.

O módulo faz a liberação no CSP (COntent Security Policy) para os hosts abaixo:

- \*.tolvnow.com
- \*.tolv.io

## Instalação

1. Acesse a raiz do seu projeto Magento 2.x e entre na pasta app/code

`~# cd app/code`

2. Baixe o projeto diretamente do repositório git:

~# git clone https://github.com/tolv12/tolv-magento-2.x.git

3. Copie o módulo para a pasta atual e remova os demais arquivos:

~# mv tolv-magento-2.x/tolv .
~# rm -rf tolv-magento-2.x

4. Volte para a pasta raiz do seu projeto Magento 2.0 e execute os comandos abaixo:

~# php bin/magento setup:upgrade
~# php bin/magento module:enable --clear-static-content Tolv_Magento2

5. Execute o comando abaixo para validar a instalação:

~# php bin/magento module:status | grep Tolv
Tolv_Magento2

Neste momento o Tolv já deve estar sendo carregado normalmente na sua loja virtual.
