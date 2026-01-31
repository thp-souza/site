# Plataforma Web Privada de Capoeira

Sistema privado para ensino de capoeira com autenticação, cordas personalizadas e gestão de conteúdo.

## 🚀 Instalação Rápida

### Pré-requisitos
- Node.js 18+ 
- npm ou yarn
- SQLite (incluso)

### Passo a Passo

1. **Clone ou baixe os arquivos**
   ```bash
   # Crie um novo diretório para o projeto
   mkdir capoeira-platform
   cd capoeira-platform
Copie todos os arquivos fornecidos para a pasta do projeto

Instale as dependências

bash
npm install
Configure o ambiente

bash
# Renomeie o arquivo .env.local.example para .env.local
# (ou crie um novo .env.local com as configurações)
Configure o banco de dados

bash
# Gere o cliente Prisma
npx prisma generate

# Execute as migrações
npx prisma db push

# Execute o seed para criar dados iniciais
npm run db:seed
Execute o servidor de desenvolvimento

bash
npm run dev
Acesse a aplicação

Abra http://localhost:3000 no navegador

🔐 Credenciais Iniciais
Administrador
Email: admin@capoeira.com

Senha: Admin123!

Aluno de Exemplo
Email: aluno@capoeira.com

Senha: User123!

📁 Estrutura do Projeto
text
capoeira-platform/
├── prisma/           # Schema do banco de dados
├── src/
│   ├── app/          # Páginas e rotas da API
│   ├── components/   # Componentes React
│   ├── lib/          # Utilitários e configurações
│   └── middleware.ts # Middleware de autenticação
└── public/           # Arquivos estáticos
🛠️ Funcionalidades
Para Administradores
✅ Criar e gerenciar usuários

✅ Criar cordas totalmente personalizadas (cor, gradiente, imagem)

✅ Organizar cordas por ordem

✅ Criar módulos/fases dentro de cada corda

✅ Adicionar movimentos com vídeos demonstrativos

✅ Dashboard administrativo completo

Para Alunos
✅ Acesso apenas à corda atribuída

✅ Visualização de módulos e movimentos da sua corda

✅ Player de vídeo integrado

✅ Interface responsiva e intuitiva

Segurança
✅ Autenticação JWT com cookies HTTP-only

✅ Middleware de proteção de rotas

✅ Acesso restrito por corda

✅ Senhas hasheadas com bcrypt

🚀 Deploy
Para produção
Configure variáveis de ambiente no servidor

Altere as chaves secretas no .env.local

Execute o build:

bash
npm run build
npm start
Recomendações para produção
Use PostgreSQL ou MySQL em vez de SQLite

Configure HTTPS

Use um CDN para vídeos

Implemente backup automático do banco

🔧 Comandos Úteis
bash
# Desenvolvimento
npm run dev

# Produção
npm run build
npm start

# Banco de dados
npx prisma studio  # Interface visual do banco
npx prisma db push # Atualizar schema

# Limpar cache
rm -rf .next node_modules
npm install
📞 Suporte
Para dúvidas ou problemas:

Verifique se todas as dependências estão instaladas

Confirme que o banco de dados foi configurado

Verifique as variáveis de ambiente

Consulte os logs do servidor

Desenvolvido para escolas e grupos de capoeira 🥋