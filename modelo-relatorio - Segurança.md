# RELATÓRIO DE IMPLEMENTAÇÃO DE MEDIDAS DE SEGURANÇA

Data: 28/01/2024
Empresa: RhoneyInc Software Full
Responsável: Ronaldo Martins

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa RhoneyInc Software Full, realizado por Ronaldo Martins. O objetivo do projeto foi elencar 3 medidas de segurança em conjunto dos serviços da AWS, com a finalidade de aumentar a segurança na empresa.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 medidas de segurança. A seguir, serão descritas as etapas da implementação:

Medida 1: 
- ## Responsabilidade compartilhada da AWS para segurança:
Com foco na segurança compartilhada, a ***AWS*** assume a responsabilidade pela segurança de sua infraestrutura e priorizou a segurança da plataforma, a fim de proteger as informações e os aplicativos críticos dos clientes.
Porém, o cliente fica responsável por garantir que o ambiente da AWS seja configurado de forma segura (o usuário deve se familiarizar com as rotinas de configurações de seguraças internas da sua empresa). Assim, para que os dados não sejam compartilhados com alguém com os quais não devem ser compartilhados, identificando quando um usuário usa indevidamente a AWS e aplicando políticas de conformidade e governança.  
### Responsabilidade da Amazon – 
*** Como tem pouco controle sobre como a AWS é usada por seus clientes, a Amazon se concentrou na segurança da infraestrutura da AWS, inclusive protegendo seus serviços de computação, armazenamento, rede e banco de dados contra intrusões. A Amazon é responsável pela segurança do software, hardware e instalações físicas que hospedam os serviços da AWS. A Amazon também se responsabiliza pela configuração de segurança de seus serviços gerenciados, como o Amazon DynamoDB, o RDS, o Redshift, o Elastic MapReduce, o WorkSpaces, dentre outros. ***
### Responsabilidade do cliente –
*** Os clientes da AWS são responsáveis ​​pelo uso seguro dos serviços da AWS considerados não gerenciados. Por exemplo, embora a Amazon tenha criado várias camadas de recursos de segurança para impedir o acesso não autorizado à AWS, incluindo a autenticação multifatorial, é responsabilidade do cliente garantir que a autenticação multifatorial esteja ativada para os usuários, especialmente para aqueles com as mais extensas permissões do IAM. ***

Medida 2: 
- ## CloudTrail:
*** O CloudTrail é um serviço da AWS que gera arquivos de log de todas as chamadas de API feitas na AWS, incluindo o console de gerenciamento, SDKs, ferramentas de linha de comando, dentre mais. ***
*** Os arquivos de log gerados são armazenados em um bucket S3 ( uma espécie de "BALDE"). Se um hacker ganhar acesso a uma conta da AWS, uma das primeiras coisas que farão é desativar o CloudTrail e excluir os arquivos de log. ***


Medida 3: 
- ## Identity and Access Management IAM:
*** Este serviço oferece  provisionamento de usuários e controle de acesso para usuários da AWS ***
*** Ao criar políticas do IAM, verifique se elas estão associadas a grupos ou funções, em vez de a usuários individuais, para minimizar o risco de um usuário individual obter permissões ou privilégios excessivos e desnecessários por acidente. ***
*** Provisionar acesso a um recurso usando funções do IAM em vez de fornecer um conjunto individual de credenciais para acesso, a fim de garantir que as credenciais perdidas ou comprometidas não levem a acesso não autorizado ao recurso. ***
*** Certifique-se de que os usuários do IAM recebam privilégios mínimos de acesso aos recursos da AWS que ainda permitam que eles cumpram suas responsabilidades de trabalho. ***


## Conclusão:
A implementação de ferramentas na empresa RhoneyInc Software Full tem como esperado aseegurar o controle, a autenticidade e o bom funcionamneto dos serviços, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.


Assinatura do Responsável pelo Projeto: Dom Carlos Borges

Ronaldo Martins