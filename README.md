# Proyecto DEOS (Decentralized Enhanced Omniscient System)

## Descripción
DEOS es un sistema de trading automatizado basado en inteligencia artificial (IA) que toma decisiones de inversión en criptomonedas utilizando más de 700 variables en tiempo real. Su objetivo es maximizar los retornos mediante un análisis profundo de datos económicos, políticos, sociales y tecnológicos, sin intervención humana.

DEOS combina análisis técnico, fundamental y de sentimiento, adaptándose continuamente a las condiciones del mercado y operando con velocidad y precisión milimétrica.

## Objetivo
Crear un bot financiero autónomo capaz de operar con múltiples criptomonedas de manera eficiente, minimizando riesgos y maximizando los beneficios a través de estrategias de trading automatizado.

### Características Clave:
- **Cobertura**: Análisis de más de 700 variables de datos en tiempo real.
- **Velocidad**: Toma de decisiones y ejecución de órdenes en milisegundos.
- **Adaptabilidad**: Reentrenamiento continuo de los modelos para adaptarse al mercado.
- **Tecnología**: LSTM, Transformers, BERT, y Reinforcement Learning para análisis avanzados.

## Estructura del Proyecto

El proyecto DEOS tiene la siguiente estructura de carpetas:

- **DEOS/**  
  El directorio raíz del proyecto.

  - **README.md**  
    Este archivo de documentación.
  
  - **requirements.txt**  
    Archivos con las dependencias del proyecto.

  - **config/**  
    Archivos de configuración.

    - **settings.yaml**  
      Configuración general del sistema.
  
    - **secrets.env**  
      Variables de entorno secretas.

  - **data/**  
    Datos recolectados.

    - **raw/**  
      Datos sin procesar.

      - **prices/**  
        Precios de criptomonedas.

      - **orderbook/**  
        Datos del libro de órdenes.

      - **volatility/**  
        Datos sobre volatilidad del mercado.

      - **liquidity/**  
        Información sobre liquidez.

      - **sentiment/**  
        Sentimiento del mercado basado en redes sociales y noticias.

        - **twitter/**  
          Datos de Twitter.

        - **reddit/**  
          Datos de Reddit.

        - **google_trends/**  
          Datos de Google Trends.

        - **telegram/**  
          Datos de Telegram.

        - **discord/**  
          Datos de Discord.

      - **news/**  
        Noticias relacionadas con el mercado.

        - **financial_news/**  
          Noticias financieras.

        - **crypto_news/**  
          Noticias sobre criptomonedas.

        - **regulation_news/**  
          Noticias sobre regulaciones.

        - **technological_news/**  
          Noticias tecnológicas.

      - **on_chain/**  
        Datos sobre la blockchain.

        - **hashrate/**  
          Datos de hashrate.

        - **wallet_flows/**  
          Flujos de carteras.

        - **miner_balances/**  
          Balances de mineros.

        - **stablecoin_supply/**  
          Suministro de stablecoins.

        - **transaction_costs/**  
          Costos de transacciones.

        - **nodes_activity/**  
          Actividad de nodos.

      - **macro/**  
        Datos macroeconómicos.

        - **inflation/**  
          Datos sobre inflación.

        - **interest_rates/**  
          Tasas de interés.

        - **unemployment/**  
          Datos sobre desempleo.

        - **economic_calendar/**  
          Calendario económico.

        - **commodity_prices/**  
          Precios de commodities.

        - **stock_indices/**  
          Índices de acciones.

      - **geopolitics/**  
        Datos geopolíticos.

        - **conflicts/**  
          Conflictos internacionales.

        - **elections/**  
          Elecciones políticas.

        - **new_regulations/**  
          Nuevas regulaciones.

        - **major_agreements/**  
          Acuerdos importantes.

      - **psychology/**  
        Psicología del mercado.

        - **fear_greed_index/**  
          Índice de miedo y codicia.

        - **public_surveys/**  
          Encuestas públicas.

        - **consumer_sentiment/**  
          Sentimiento del consumidor.

      - **technology/**  
        Datos sobre tecnología.

        - **github_activity/**  
          Actividad en GitHub.

        - **patents/**  
          Patentes tecnológicas.

        - **ai_innovations/**  
          Innovaciones en IA.

      - **energy/**  
        Datos sobre energía.

        - **electricity_prices/**  
          Precios de electricidad.

        - **mining_energy_usage/**  
          Uso de energía en minería.

        - **renewable_energy_trends/**  
          Tendencias de energía renovable.

      - **anomalies/**  
        Datos sobre anomalías en el mercado.

        - **flash_crashes/**  
          Caídas repentinas del mercado.

        - **hack_reports/**  
          Informes sobre hackeos.

        - **regulatory_cracks/**  
          Fallos regulatorios.

        - **security_alerts/**  
          Alertas de seguridad.

      - **meteorology/**  
        Datos meteorológicos.

        - **mining_regions_weather/**  
          Clima en regiones mineras.

        - **disaster_alerts/**  
          Alertas de desastres.

    - **processed/**  
      Datos ya procesados.

      - **consolidated/**  
        Datos consolidados.

      - **backup_versions/**  
        Versiones de respaldo de los datos.

    - **features/**  
      Características extraídas de los datos.

      - **technical/**  
        Indicadores técnicos.

      - **sentiment_scores/**  
        Puntuaciones de sentimiento.

      - **macro_features/**  
        Características macroeconómicas.

      - **onchain_features/**  
        Características de la blockchain.

      - **risk_indicators/**  
        Indicadores de riesgo.

      - **custom_indicators/**  
        Indicadores personalizados.

  - **notebooks/**  
    Notebooks de análisis y pruebas.

  - **src/**  
    Código fuente del proyecto.

    - **data_collection/**  
      Scripts para recolectar los datos.

    - **preprocessing/**  
      Scripts para el procesamiento de los datos.

    - **models/**  
      Modelos de IA, como LSTM, Transformers, etc.

    - **decision_engine/**  
      Lógica para la toma de decisiones de compra/venta.

    - **trading_execution/**  
      Ejecución de órdenes en exchanges.

    - **monitoring/**  
      Monitoreo y seguimiento del desempeño de los bots.

  - **bots/**  
    Archivos y scripts relacionados con los bots de trading.

  - **models/**  
    Modelos entrenados y sus componentes.

    - **saved_models/**  
      Modelos guardados.

    - **scalers/**  
      Escaladores de datos para el preprocesamiento.

  - **logs/**  
    Archivos de logs generados por el sistema.

    - **training_logs/**  
      Logs de entrenamiento de los modelos IA.

    - **trading_logs/**  
      Logs de las operaciones de trading.

    - **error_logs/**  
      Logs de errores del sistema.

  - **tests/**  
    Pruebas unitarias y de integración del proyecto.

  - **deployments/**  
    Archivos para el despliegue del sistema.

    - **docker-compose.yml**  
      Configuración de Docker Compose para el entorno de despliegue.

    - **deploy_local.sh**  
      Script para desplegar localmente el proyecto.

    - **deploy_server.sh**  
      Script para desplegar en el servidor.
