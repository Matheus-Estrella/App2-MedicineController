💊 Medicine Controller
Um aplicativo mobile para controle de medicamentos desenvolvido em React Native com Expo, featuring autenticação de usuários e CRUD completo de medicamentos integrado com API externa.

📋 Funcionalidades
🔐 Autenticação Segura: Sistema de login com credenciais protegidas

💊 Gerenciamento de Medicamentos: CRUD completo (Criar, Ler, Atualizar, Excluir)

📱 Interface Intuitiva: Design moderno com navegação fluida

☁️ Persistência em Nuvem: Integração com MockAPI para armazenamento

⚡ Desempenho Otimizado: Carregamento rápido e experiência responsiva

🚀 Pré-requisitos
Antes de começar, verifique se você tem instalado em sua máquina:

Node.js (versão 16 ou superior) - Download aqui

Git - Download aqui

Expo Go (no smartphone) - Android ou iOS

📥 Instalação Passo a Passo
1. Clone o repositório
bash
git clone https://github.com/Matheus-Estrella/App2-MedicineController.git
cd App2-MedicineController
2. Instale as dependências
bash
npm install
3. Instale as dependências específicas do Expo
bash
npx expo install @react-navigation/native @react-navigation/stack react-native-screens react-native-safe-area-context axios @expo/vector-icons @react-native-async-storage/async-storage
🏃‍♂️ Executando o Projeto
Para desenvolvimento:
bash
npx expo start
Comandos úteis:
bash
# Limpar cache (se necessário)
npx expo start --clear

# Executar em modo específico
npx expo start --android    # Android
npx expo start --ios        # iOS (requer Mac)
npx expo start --web        # Navegador web
📱 Como testar no smartphone:
Abra o app Expo Go no seu celular

Escaneie o QR code que aparece no terminal

Aguarde o carregamento do aplicativo

🔐 Credenciais de Teste
Use as seguintes credenciais para fazer login:

Usuário: admin

Senha: admin1234

🛠️ Tecnologias Utilizadas
React Native - Framework para aplicativos móveis

Expo - Plataforma para desenvolvimento React Native

TypeScript - JavaScript com tipagem estática

React Navigation - Navegação entre telas

Axios - Cliente HTTP para APIs

AsyncStorage - Armazenamento local

MockAPI - API REST para persistência de dados

📊 API Integration
O projeto utiliza API externa para persistência de dados:

💊 Medicamentos (MockAPI)
URL: https://68d1871be6c0cbeb39a51abd.mockapi.io/api/v1/medicines

Função: CRUD completo de medicamentos (GET, POST, PUT, DELETE)

🎯 Funcionalidades Detalhadas
1. Sistema de Autenticação
Login com usuário e senha local

Armazenamento seguro de token com AsyncStorage

Logout com confirmação

Navegação condicional automática

2. Gerenciamento de Medicamentos
Cadastrar: Formulário com validação (nome, dosagem, horário, observações)

Listar: Visualização em cards com FlatList e pull-to-refresh

Editar: Formulário pré-preenchido para alterações

Excluir: Modal de confirmação antes da exclusão

3. Interface do Usuário
Design responsivo e intuitivo

Componentes modulares reutilizáveis

Ícones e feedback visual

Loading states durante operações assíncronas

Mensagens de erro e sucesso

🐛 Solução de Problemas Comuns
Erro de Cache do Metro Bundler
bash
npx expo start --clear
Dependências corrompidas
bash
rm -rf node_modules
rm package-lock.json
npm install
Erro de tipo TypeScript
bash
npx tsc --noEmit
Aplicativo não carrega
Verifique se o arquivo App.tsx existe na raiz

Confirme se todas as importações estão corretas

Execute npx expo start --reset-cache

Problemas de navegação
Verifique se todas as telas estão registradas no App.tsx

Confirme os nomes das rotas nas navegações

📝 Scripts Disponíveis
bash
npm start          # Inicia o servidor de desenvolvimento
npm run android    # Executa no Android
npm run ios        # Executa no iOS (apenas Mac)
npm run web        # Executa no navegador

