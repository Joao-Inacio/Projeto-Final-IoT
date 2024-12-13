# **🌤️ Estação Meteorológica Inteligente**

Este é o projeto final do curso de Automação com IoT, onde foi desenvolvida uma Estação Meteorológica Inteligente simulada. O projeto utiliza sensores virtuais para monitorar condições ambientais e exibir os dados em tempo real através de gráficos e uma aplicação web personalizada.

## 📋 Descrição

A Estação Meteorológica Inteligente foi projetada para simular a coleta e análise de dados ambientais, integrando conceitos de Internet das Coisas (IoT), protocolo MQTT, plataformas de simulação, e desenvolvimento web. O objetivo é demonstrar como tecnologias acessíveis podem ser usadas para criar soluções inteligentes e conectadas.

- **[Link da apresentação](https://drive.google.com/file/d/11hjlodeT9Pxh_ZKepzQFEhfrBXtVHys4/view?usp=drive_link)** 

## 🛠️ Ferramentas e Tecnologias Utilizadas
- **Simulação e Sensores**
    - Wokwi.com: Plataforma para simulação do hardware, incluindo o ESP32 e os sensores.
    Módulo DHT22: Para medir temperatura e umidade.
    LDR (Light Dependent Resistor): Para medir luminosidade.
- **Conexão e Armazenamento**
    - Protocolo MQTT: Para envio dos dados coletados.
    - ThingSpeak: Para armazenar, exibir gráficos em tempo real e disponibilizar uma API para integração.
- **Desenvolvimento Web**
    - Python e Flask: Para criar uma aplicação web que exibe os gráficos e informações coletadas diretamente do ThingSpeak.
    - 
## **🚀 Funcionalidades**

Simulação de coleta de dados ambientais usando o Wokwi.com.
Monitoramento de temperatura, umidade e luminosidade.
Envio de dados via protocolo MQTT para o ThingSpeak.
Visualização de gráficos atualizados em tempo real no ThingSpeak.
Aplicação web personalizada que exibe os gráficos e dados integrados.

## **📂 Estrutura do Projeto**

```bash
.
├── app.py                # Código principal da aplicação Flask
├── templates/
│   └── index.html        # Página principal da aplicação web
├── static/               # Imagens do gráficos 

├── README.md             # Documentação do projeto
└── requirements.txt      # Dependências do projeto
```

## 📡 Configuração e Execução

- Pré-requisitos
    - Python 3.7+
    - Conta no ThingSpeak
    - Biblioteca do Python:
      - Flask

**Instalação**
---
**Clone o repositório:**

```bash
git clone https://github.com/Joao-Inacio/Projeto-Final-IoT
cd estacao-meteorologica-inteligente
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

**Configure o ThingSpeak:**

Insira as credenciais do canal, como CHANNEL_ID e READ_API_KEY, no arquivo app.py.
Inicie o servidor Flask:


```bash
python app.py
```

**Acesse a aplicação no navegador:**


http://127.0.0.1:5000

**📊 Visualização no ThingSpeak**
---
Gráficos em Tempo Real:[ Link do canal público no ThingSpeak.](https://thingspeak.mathworks.com/channels/2720534)
Integração via API para exibir gráficos personalizados na aplicação Flask.

## **🎯 Próximos Passos**

Melhorar o Design: Personalizar ainda mais a interface da aplicação web.
Adicionar Previsões: Futuras implementações de Machine Learning para prever dados ambientais.
📄 Licença
Este projeto está licenciado sob a MIT License.

## **✨ Créditos**

Projeto desenvolvido por João Inácio como parte do curso de Automação com IoT.
