# RPA Suprimentos - Challenge

O projeto é focado no gerenciamento de suprimentos de uma empresa, envolvendo a extração e preenchimento dos campos requisitados com informações detalhadas sobre os produtos adquiridos, sempre considerando o PO (Purchase Order) específico de cada estado dos Estados Unidos.

### Tecnologias Utilizadas

Para esse projeto, algumas tecnologias foram utilizadas:

* [Automation Anywhere](https://www.automationanywhere.com/)
* [Excel]()

## 📌 Informações importantes sobre a aplicação

* Como o projeto foi desenvolvido na plataforma AA 360 University, não é possível compartilhar o projeto diretamente com terceiros.
* O projeto ainda está em fase de melhorias. Sugestões são aceitas e podem ser enviadas para o e-mail marthabeatrizsiq@gmail.com.

## ⏭️ Próximos passos

1.0 Implementar novas ações que verificam se o usuário já está logado nas aplicações que são utilizadas. ✅<br/>
2.0 Implementar ações de envio de e-mail contendo as ordens de compras processadas por execução. ✅ <br/>

## Considerações sob as mudanças
 
_1.0 Implementar novas ações que verificam se o usuário já está logado nas aplicações que são utilizadas_

Para as aplicações web utilizadas, foi implementada uma lógica com um pacote de ações de gerenciamento de erros. A lógica verifica se a janela de Login está disponível. Caso positivo, as credenciais do usuário são inseridas e validadas antes de prosseguir para as etapas seguintes do código.

![image](https://github.com/user-attachments/assets/2f35ac2e-c840-4ff2-91f2-08c843d26a7d)

Caso ocorra um erro durante o Login, uma mensagem de exceção será registrada e o e-mail correto será enviado ao usuário.

![image](https://github.com/user-attachments/assets/4f545d9e-9653-41ee-aa24-0bfd0d1b5d9f)

_2.0 Implementar ações de envio de e-mail contendo as ordens de compras processadas por execução_

Se a mensagem de erro estiver vazia e a linha de erro for igual a 0, um e-mail de sucesso deverá ser enviado, incluindo uma tabela com todas as ordens de compra e a data de execução.

![image](https://github.com/user-attachments/assets/5349e884-44a3-49cf-8dfe-30a3b3184bd9)

Caso contrário, um e-mail de erro será enviado contendo, em detalhes, as informações sobre o erro ocorrido durante a execução.

![image](https://github.com/user-attachments/assets/231f3812-6af6-4f8b-8c98-843268834a3c)
