# 🚀 Mission Control IA - Monitoramento Espacial FIAP

## 📋 Integrantes e RM
* **Nome Completo:** Kauan Damasceno de Lima - **RM:** 573727
* **Nome Completo:** Thiago Soalheiro Diamantino - **RM:** 569316

---

## 🛰️ O que o projeto faz e seu Objetivo
Este projeto foi desenvolvido como parte da **Global Solution 2026** da FIAP para a disciplina *Prompt and Artificial Intelligence*. 

O objetivo principal é simular o sistema de controle e telemetria de uma missão aeroespacial experimental. O software utiliza Inteligência Artificial Generativa local através do modelo **Llama 3.2 1B** (via Ollama) para realizar o sorteio interno de dados críticos de voo, validar regras operacionais de segurança de hardware e fornecer diagnósticos preditivos acionáveis em tempo real para a tripulação técnica.

---

## 🛠️ Tecnologias Utilizadas
* **Python 3** (Lógica estrutural e exibição de dados)
* **Ollama API** (Gerenciamento e execução do LLM local no ambiente de nuvem)
* **Llama 3.2 1B** (Modelo de linguagem natural especializado em análise preditiva espacial)
* **Google Colab Notebook** (Ambiente de desenvolvimento e execução)

---

## 📊 Parâmetros Monitorados e Regras de Negócio
O sistema analisa de forma autônoma os seguintes componentes da nave:

1. **Temperatura:** Faixa de 10°C a 110°C. Dispara aviso crítico se ultrapassar 80°C.
2. **Energia Global:** Faixa de 1% a 100% de bateria. Emite alertas específicos para nível baixo (11% a 20%) e nível crítico (menor ou igual a 10%).
3. **Link de Comunicação:** Classificado entre Estável, Instável, Crítico ou Desconectado. Dispara alerta de reconexão obrigatória caso o sinal fique Crítico ou Desconectado.
4. **Status dos Módulos:** Monitora se os subsistemas estão Ativos ou Inativos, alertando falha se houver inatividade.

---

## 📸 Demonstração do Sistema Operando - Em Prints

### 🟢 1. Cenário Operacional Normal (Sem Alertas)
![Dados da missão](assets/dados_missao.png)

### 🔴 2. Cenário Operacional Crítico (Alertas Ativados pelo Llama)
![Alerta critico](assets/alerta_critico.png)

---

## Como Executar o Projeto

Todo o projeto foi estruturado para rodar 100% em nuvem através do Google Colab, eliminando qualquer necessidade de instalações locais complexas.

1. **Acesse o Notebook:** [CLIQUE AQUI PARA ACESSAR O GOOGLE COLAB](https://colab.research.google.com/drive/1pE5grIonkj6OZMGy9CkkHAiicktkT8wJ?usp=sharing)
2. **Configuração do Ambiente:** Execute a primeira célula do script para baixar, configurar a engine do Ollama em background e fazer o pull do modelo `llama3.2:1b`.
3. **Geração e Relatório:** Execute a célula do prompt de controle. O painel gráfico estruturado e a resposta preditiva da IA serão impressos diretamente no console de saída.

---

## 🎥 Vídeo de Demonstração
Um vídeo explicativo com duração máxima de 3 minutos está disponível no link abaixo, apresentando os integrantes do grupo, explicando a arquitetura adotada do prompt e demonstrando a IA rodando cenários críticos ao vivo:

▶️ [Assista ao Vídeo de Demonstração no YouTube]() 
