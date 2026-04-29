# REGA-MAPA Digital Twin Dashboard 🌿
Interface de monitoramento e controle em tempo real para o ecossistema REGA V4.2.

## 🚀 Como Funciona
Este dashboard é uma aplicação "Static Web App" hospedada via **GitHub Pages**. Ele funciona como um "Digital Twin" (Gêmeo Digital) do seu sistema físico, comunicando-se diretamente com o seu **REGA LINK Gateway** local.

### Diferenciais desta Versão
- **Hybrid Cloud:** O rádio cuida apenas dos dados (leve), enquanto o GitHub entrega a interface (pesado).
- **Sem SD Busy:** Elimina travamentos de leitura no cartão SD do ESP32.
- **Performance:** Gráficos de 24h e monitoramento de múltiplos hubs simultâneos.

## 🛠️ Configuração Rápida
1. Ao abrir o dashboard pela primeira vez, ele solicitará o **IP Local** do seu Gateway (ex: `192.168.1.53`).
2. O navegador salvará esse IP automaticamente (via LocalStorage).
3. Certifique-se de que seu celular/PC esteja na mesma rede Wi-Fi que o REGA LINK.

## 📡 Arquitetura do Sistema
- **Frontend:** HTML5, CSS3 e JavaScript (Chart.js) via GitHub Pages.
- **Data Source:** ESP32 REGA LINK (Endpoints: `/topology`, `/history`, `/uptime`).
- **Comunicação:** Protocolo REGA V4 (LoRa 915MHz).

---
*Desenvolvido para o monitoramento avançado de sistemas de irrigação automatizados.*
