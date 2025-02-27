A aplicação contém um cadastro de usuários para efetuar o login em uma determinada página.Ela contém:

**HASH DE SENHA: Que serve para proteger a senha de possivéis invasores dentro do banco de dados ,o HASH transforma uma senha simples em códigos, ele utiliza caracteres comuns e especiais dificultando o trabalho de possivéis invasores tornando quase impossível descobrir a senha verdadeira do usuário.

**PHPMailer: é uma biblioteca popular para PHP que simplifica o envio de e-mails. Ele oferece uma interface fácil de usar e recursos avançados, como suporte a SMTP, anexos e HTML.Nesse caso usamos ela para fazer o envio do código de validação,o usuário cadastra o email, e no mesmo momento um código e enviado para o email cadastrado esse código quem é o responsável por libera o acesso ao programa.

CONFIGURAÇÃO DO EMAIL:
1º ACESSE SEU EMAIL, VÁ ATÉ SEU PERFIL DO GOOGLE (OU FOTO) NO CANTO DIREITO DA TELA E CLIQUE EM GERENCIAR SUA CONTA DO GOOGLE.
2° CLIQUE EM SEGURANÇA.
3° LIBERE PARA A VERIFICAÇÃO EM DUAS ETAPAS.
4° VAI LIBERAR E GERAR UM CÓDIGO DE 16 DIGITOS, ESSE CÓDIGO VAI SER INSERIDO NA SUA LINHA DE N° 19 NO CÓDIGO.



CONFIGURAÇÃO DO CÓDIGO PARA O FUNCIONAMENTO:
1º VÁ ATÉ A PÁGINA MAIL.PHP 

   linhas 18 ->     $mail->Username = 'digite o email de envio'; //Preencher com e-mail para envio
   linhas 19 ->     $mail->Password = 'senha app 16 caracteres.'; //Preencher a senha do app com o código gerado no seu email.

   linhas 28 ->     $mail->setFrom('digite o email de envio', 'nome da aplicação'); //Preencher com e-mail para envio

   Essas são as configurações necessárias no código, o email pode ser qualquer um que o usuário no caso o progrmador tem acesso, pois ele vai ter que acessar o gmail.
  


