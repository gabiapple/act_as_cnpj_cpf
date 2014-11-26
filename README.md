# act_as_cnpj_cpf

[![Build Status](https://travis-ci.org/josuelima/act_as_cnpj_cpf.svg?branch=master)](https://travis-ci.org/josuelima/act_as_cnpj_cpf)
[![Code Climate](https://codeclimate.com/github/josuelima/act_as_cnpj_cpf/badges/gpa.svg)](https://codeclimate.com/github/josuelima/act_as_cnpj_cpf)
[![Test Coverage](https://codeclimate.com/github/josuelima/act_as_cnpj_cpf/badges/coverage.svg)](https://codeclimate.com/github/josuelima/act_as_cnpj_cpf)

** Rubygem to format and validate CNPJ (Brazilian company registration number) and CPF (Brazilian citizens registration number). You can use it solo or as an ActiveRecord plugin. **

act_as_cnpj_cpf é uma Rubygem para validar e formatar CNPJ e CPF.

## Funcionalidades:

* Valida CPF e CNPJ com ou sem formatação
* Integração com ActiveRecord
* Formata número para o padrão do CNPJ ou CPF (xx.xxx.xxx/xxxx-xx e xxx.xxx.xxx-xx)
* Possibilidade de utilizar um atributo como CNPJ ou CPF ao mesmo tempo
* Permite persistir cpf ou cnpj inválido (caso seja especificado com permite_invalido: true)

Este projeto foi inicialmente desenvolvido como uma extensão da gem [brcpfcnpj](https://github.com/tapajos/brazilian-rails/tree/master/brcpfcnpj) e em seguida totalmente re-escrito por se tratar de uma proposta diferente. Além das novas funcionalidades, diferentemente do brcpfcnpj, este projeto utiliza o número sem formatação como padrão para salvar no banco de dados e exibir (podendo ser exibido formatado com .formatado)