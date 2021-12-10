# react_twilio
App de chat utilizando sdk e api da twilio

## SDK Twiliio

para o correto funcionamento, startar o sdk da twilio, para isso faça clone do projeto

```bash
git clone https://github.com/TwilioDevEd/sdk-starter-node.git
```

Entre na pasta do proejto, instale todas as dependencias e para o funcionamento junto a essa aplicação instale também a biblioteca cors:
```bash
cd sdk-starter-node
npm install
npm install cors
```

Atualize o arquivo _app.js_ adicionando as linhas abaixo:
```javascript
const app = express();
const cors = require('cors');
app.use(cors());
```

Na sequência faça uma copia do arquivo _.env.example_
```bash
mv .env.example .env
```

Adicione os valores das chave:
- TWILIO_ACCOUNT_SID
- TWILIO_API_KEY
- TWILIO_API_SECRET

> Exclua as outras chaves que não serão utilizadas.

Na sequência execute a aplicação numa porta diferente da 3000:
```bash
PORT=5000 npm start
```

