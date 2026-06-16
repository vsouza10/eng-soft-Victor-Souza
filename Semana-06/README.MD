# Victor Emanuel de Souza

## Engenharia de Software

# Conversa com o Cliente – Hotel Bela Vista

## Entrevista

### Analista (Victor)

Olá! Tudo bem? Meu nome é Victor, sou analista de sistemas e estou aqui para entender melhor seu negócio e como posso te ajudar.

### Cliente

Olá, Victor! Tudo bem, não está, mas vamos levando. O hotel cresceu e estou com dificuldades para organizar as reservas.

### Analista

Entendo. Como você faz esse controle hoje?

### Cliente

Uso um caderno grande. Faço uma tabela com dias e quartos e anoto tudo à mão.

### Analista

E quais problemas você enfrenta?

### Cliente

Vários:

- Rasuras quando alguém cancela.
- Esquecimento de dados como CPF.
- Confusão com tipos de quartos.
- Reservas duplicadas.
- Perda de informações em papéis soltos.

### Analista

Quantos quartos você tem atualmente?

### Cliente

30 quartos, com tipos diferentes: simples, luxo e família.

### Analista

Você trabalha sozinho?

### Cliente

Não. Minha filha e um funcionário também ajudam, mas cada um escreve de um jeito.

### Analista

Você utiliza computador?

### Cliente

Sim, prefiro o computador por causa da tela maior.

### Analista

Você gostaria de um sistema com um painel visual dos quartos?

### Cliente

Sim! Algo que eu olhe e já entenda tudo.

### Analista

E controle de consumo dos hóspedes?

### Cliente

Seria essencial. Já perdi dinheiro com isso.

### Analista

Perfeito. Vou organizar isso em funcionalidades e te apresento.

---

# Histórias de Usuário

- **HU01:** Como recepcionista, quero visualizar todos os quartos em uma tela com cores para identificar rapidamente o status de cada um.
- **HU02:** Como recepcionista, quero registrar reservas sem risco de sobrescrever outras.
- **HU03:** Como recepcionista, quero cadastrar hóspedes com nome, telefone e CPF.
- **HU04:** Como recepcionista, quero visualizar entradas e saídas do dia.
- **HU05:** Como recepcionista, quero registrar consumo de produtos por hóspede.
- **HU06:** Como recepcionista, quero calcular automaticamente o valor total no checkout.
- **HU07:** Como dono do hotel, quero eliminar o uso de papel para evitar perda de informações.
- **HU08:** Como usuário, quero um sistema simples e fácil de usar.

---

# Validação

### Analista

Essas funcionalidades representam o que você precisa?

### Cliente

Sim, isso resolve meus problemas.

---

# Requisitos Funcionais

- **RF01:** O sistema deve exibir um painel com todos os quartos e seus status (livre, ocupado e limpeza).
- **RF02:** O sistema deve permitir o cadastro de reservas.
- **RF03:** O sistema deve impedir reservas duplicadas para o mesmo quarto no mesmo período.
- **RF04:** O sistema deve permitir o cadastro completo de hóspedes (nome, telefone e CPF).
- **RF05:** O sistema deve exibir entradas e saídas do dia.
- **RF06:** O sistema deve permitir o registro de consumo por hóspede.
- **RF07:** O sistema deve calcular automaticamente o valor total no checkout.

---

# Requisitos Não Funcionais

- **RNF01:** O sistema deve ser acessível via computador.
- **RNF02:** O sistema deve possuir interface simples e intuitiva.
- **RNF03:** O sistema deve responder em até 2 segundos.
- **RNF04:** O sistema deve utilizar cores para facilitar a visualização dos status dos quartos.

---

# Regras de Negócio

- **RN01:** Um quarto não pode ser reservado por mais de um hóspede no mesmo período.
- **RN02:** O cadastro do hóspede deve conter CPF obrigatório.
- **RN03:** Todo consumo deve ser vinculado ao hóspede durante a estadia.
