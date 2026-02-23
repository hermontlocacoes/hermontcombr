# Instruções de Deploy: Versão "Sem Instalação" (Standalone)

Como você não tem permissão de administrador para instalar o Node.js, a melhor solução é usar o **executável independente** do Firebase.

### Passo 1: Preparar o Executável
1. Pegue o arquivo que você baixou (provavelmente chamado `firebase-tools-instant-win.exe`).
2. **Renomeie** o arquivo para `firebase.exe` (apenas para facilitar).
3. **Mova** esse arquivo para dentro da pasta do seu projeto:
   `c:\Projetos python\Hermont\`

### Passo 2: Executar Comandos
Agora, em vez de usar apenas `firebase`, você precisará dizer ao terminal onde o arquivo está.

Abra o terminal na pasta do projeto e use `.\firebase` (ponto e barra invertida antes do nome):

1. **Login** (Faça uma vez):
   ```powershell
   .\firebase login
   ```
   *Isso abrirá o navegador para você autorizar.*

2. **Deploy** (Sempre que quiser atualizar o site):
   ```powershell
   .\firebase deploy
   ```

### Solução de Problemas
- Se o PowerShell bloquear a execução, tente abrir o "Prompt de Comando" (CMD) normal e digite apenas `firebase login` (estando na mesma pasta).
- Certifique-se de que o arquivo `firebase.exe` está na mesma pasta onde você abriu o terminal.
