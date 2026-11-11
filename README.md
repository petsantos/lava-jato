# 🚗 LavaJato Pro - Sistema de Gestão de Fila e Agendamentos

LavaJato Pro é uma solução completa para automação de logística de lava-jatos, focada em previsibilidade de entrega e gestão eficiente de fluxo de veículos.

## 🌟 Funcionalidades Principais

- **Dashboard Operacional**: Gestão de fila em tempo real com 6 slots de atendimento.
- **Inteligência de Fila**: Cálculo automático de previsão de entrega baseado em baias paralelas e duração dos serviços.
- **Cadastro de Clientes**: Registro de clientes com busca rápida via placa.
- **Catálogo de Serviços**: Gestão de serviços com tempos de execução definidos.
- **Controle de Status**: Fluxo de trabalho fluido: `Agendado` $\rightarrow$ `Em Lavagem` $\rightarrow$ `Concluído`.
- **Regras de Negócio**: Trava de cancelamento (mínimo 5h de antecedência) e limite estrito de capacidade.

## 🛠️ Tecnologias Utilizadas

- **Frontend**: React.js, Tailwind CSS.
- **Backend**: Node.js, Express.
- **Banco de Dados**: MySQL.

## 🚀 Como Executar o Projeto

### Pré-requisitos
- Node.js instalado.
- MySQL Server instalado e rodando.

### Instalação

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/seu-usuario/lava-jato-pro.git
   cd lava-jato-pro
   ```

2. **Configuração do Banco de Dados**:
   - Execute o arquivo `schema.sql` no seu MySQL para criar as tabelas.
   - (Opcional) Execute `seed.sql` para popular dados iniciais.

3. **Configuração do Backend**:
   - Crie um arquivo `.env` na raiz com as seguintes variáveis:
     ```env
     DB_HOST=localhost
     DB_USER=seu_usuario
     DB_PASSWORD=sua_senha
     DB_NAME=lavajato
     PORT=3001
     ```
   - Instale as dependências e inicie:
     ```bash
     npm install
     node server.js
     ```

4. **Configuração do Frontend**:
   - Acesse a pasta do frontend:
     ```bash
     cd lava-jato-frontend
     npm install
     npm run dev
     ```
   - Abra o link fornecido (ex: `http://localhost:5173`).

## 📐 Arquitetura
O projeto segue o padrão **MVC (Model-View-Controller)** no backend para garantir escalabilidade e manutenção simplificada.
