# 🔄 Tab Rotator - Extensão do Chrome

Uma extensão para o Google Chrome que alterna automaticamente entre abas em loop com tempo configurável.

## ✨ Funcionalidades

- **Rotação Automática**: Alterna entre todas as abas abertas em loop
- **Tempo Configurável**: Define o tempo de exibição de cada aba (1-300 segundos)
- **Controle Simples**: Botões para iniciar e parar a rotação
- **Interface Moderna**: Design elegante e responsivo
- **Persistência**: Mantém as configurações mesmo após fechar o navegador
- **Contador de Abas**: Mostra quantas abas estão disponíveis para rotação

## 🚀 Instalação

### Método 1: Carregar Extensão Descompactada (Recomendado para Desenvolvimento)

1. Abra o Google Chrome
2. Digite `chrome://extensions/` na barra de endereços
3. Ative o "Modo do desenvolvedor" no canto superior direito
4. Clique em "Carregar sem compactação"
5. Selecione a pasta desta extensão
6. A extensão será instalada e aparecerá na barra de ferramentas

### Método 2: Instalação via Chrome Web Store (Futuro)

*Esta extensão será disponibilizada na Chrome Web Store em breve.*

## 📖 Como Usar

1. **Abra várias abas** no seu navegador
2. **Clique no ícone da extensão** na barra de ferramentas
3. **Configure o tempo** de exibição por aba (em segundos)
4. **Clique em "Iniciar"** para começar a rotação
5. **Clique em "Parar"** para interromper a rotação

### Configurações

- **Tempo por aba**: 1-300 segundos (padrão: 5 segundos)
- **Abas incluídas**: Todas as abas normais (exclui abas do Chrome e extensões)
- **Loop contínuo**: A rotação continua indefinidamente até ser parada

## 🛠️ Estrutura do Projeto

```
tab-rotator/
├── manifest.json          # Configuração da extensão
├── popup.html             # Interface do usuário
├── popup.js               # Lógica da interface
├── background.js          # Service worker (lógica principal)
├── icons/                 # Ícones da extensão
│   └── icon.svg           # Ícone SVG
└── README.md              # Este arquivo
```

## 🔧 Tecnologias Utilizadas

- **Manifest V3**: Versão mais recente do sistema de extensões do Chrome
- **Service Workers**: Para execução em segundo plano
- **Chrome Tabs API**: Para gerenciar abas
- **Chrome Storage API**: Para persistir configurações
- **HTML5/CSS3**: Interface moderna e responsiva
- **JavaScript ES6+**: Lógica da aplicação

## 🎨 Personalização

### Modificar o Tempo Padrão

Edite o arquivo `popup.html` e altere o valor padrão no input:

```html
<input type="number" id="interval" min="1" max="300" value="5">
```

### Alterar Cores

Modifique as variáveis CSS no arquivo `popup.html`:

```css
body {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

## 🐛 Solução de Problemas

### A extensão não alterna as abas
- Verifique se há abas abertas (excluindo abas do Chrome)
- Certifique-se de que a extensão tem permissão para acessar abas
- Recarregue a extensão em `chrome://extensions/`

### A rotação para inesperadamente
- Verifique se alguma aba foi fechada durante a rotação
- A extensão se ajusta automaticamente quando abas são adicionadas/removidas

### Interface não carrega
- Verifique se todos os arquivos estão presentes
- Recarregue a extensão em `chrome://extensions/`

## 📝 Logs de Desenvolvimento

Para ver os logs da extensão:

1. Abra o DevTools (F12)
2. Vá para a aba "Console"
3. Selecione "Tab Rotator" no dropdown de contexto
4. Os logs aparecerão durante a execução

## 🤝 Contribuição

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature
3. Faça commit das suas mudanças
4. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## 🆘 Suporte

Se você encontrar algum problema ou tiver sugestões:

1. Abra uma issue no repositório
2. Descreva o problema detalhadamente
3. Inclua informações sobre seu sistema e versão do Chrome

---

**Desenvolvido com ❤️ para melhorar sua experiência de navegação!** 