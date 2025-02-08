# formulario_validacao
Formulário de Cadastro com Validações


1. Estrutura do Formulário:
O formulário deve ser dividido em, pelo menos, três seções:

Informações Pessoais:

Nome Completo
Data de Nascimento
CPF
Telefone Fixo (com DDD)
Celular (com DDD)
Informações Complementares (para menores de idade):

Se o usuário for menor de 18 anos, os campos obrigatórios devem incluir:
Nome do Pai
Nome da Mãe
Endereço:

CEP
Endereço
Número
Complemento (opcional)
Cidade
Estado
Informações da Conta:

Email
Senha
Confirmar Senha


2. Requisitos de Validação:
Cada campo do formulário deve ser validado em tempo real, fornecendo feedback visual (ex.: alteração de borda, mensagem de erro) quando os dados forem inválidos. As validações devem incluir:

Nome Completo:

Não pode ser vazio; deve conter pelo menos dois nomes (nome e sobrenome).
Data de Nascimento:

Deve ser inserida em formato DD/MM/AAAA ou outro padrão coerente.
Deve ser validada para garantir que seja uma data válida.
Calcular a idade com base na data informada.
Se a idade for menor que 18 anos, os campos de Nome do Pai e Nome da Mãe tornam-se obrigatórios.
CPF:

Deve seguir o formato “XXX.XXX.XXX-XX” ou apenas números (11 dígitos).
Implementar a validação do CPF utilizando o algoritmo de verificação dos dígitos verificadores.
Telefone Fixo:

Deve incluir o DDD e o número, no formato:
Exemplo: (11) 2345-6789
Validar se o número possui 10 dígitos (incluindo o DDD) e se a formatação está correta.
Celular:

Também deve incluir o DDD e o número, mas com o nono dígito obrigatório:
Exemplo: (11) 91234-5678
Validar se o número possui 11 dígitos (incluindo o DDD) e se a formatação está correta.
CEP:

Deve seguir o padrão “XXXXX-XXX” ou conter exatamente 8 dígitos numéricos.
Validar se o CEP possui a formatação correta.
Email:

Validar se o formato do email é válido (exemplo: “usuario@dominio.com”).
Senha:

Deve ter no mínimo 8 caracteres; preferencialmente, conter letras maiúsculas, minúsculas, números e caracteres especiais.
Fornecer feedback se a senha não atingir os critérios de segurança.
Confirmar Senha:

Deve ser idêntico ao campo de senha.
Campos para Menores de Idade (Nome do Pai e Nome da Mãe):

Se a data de nascimento indicar que o usuário possui menos de 18 anos, esses campos devem se tornar obrigatórios e não podem ser vazios.
