Padrões aplicados:
Componente	Padrão de Projeto	Finalidade
Gerenciamento de conexão DB	Singleton	Uma única instância para toda a aplicação
Lógica de cálculo de frete	Strategy	Fretes por Correios, Transportadora, Motoboy
Integração com gateways de pagamento	Facade	Esconder a complexidade de múltiplos serviços de pagamento
Criação de objetos Pedido	Builder	Construção de pedidos complexos com muitos atributos
Notificação do cliente	Observer	Enviar e-mail, SMS ou WhatsApp ao mudar o status do pedido

📁 Estrutura de Pacotes Sugerida
plaintext
Copiar
Editar
com.seuprojeto
├── Main.java
├── pedido
│   ├── Pedido.java
│   ├── PedidoBuilder.java
│   ├── PedidoStatus.java
├── frete
│   ├── FreteStrategy.java
│   ├── CorreiosFrete.java
│   ├── MotoboyFrete.java
├── pagamento
│   ├── PagamentoFacade.java
│   ├── PayPalService.java
│   ├── PicPayService.java
├── notificacao
│   ├── Notificador.java
│   ├── EmailService.java
│   ├── SmsService.java
