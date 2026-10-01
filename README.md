# WinHealth: Ferramenta de Manutenção do Windows 🛠️
WinHealth é um script de automação em Batch criado para facilitar a manutenção preventiva do Windows.

[![Batch](https://img.shields.io/badge/Batch-Script-4D4D4D?logo=windows&logoColor=white)](https://learn.microsoft.com/windows-server/administration/windows-commands/windows-commands)
[![PowerShell](https://img.shields.io/badge/PowerShell-5.1-5391FE?logo=powershell&logoColor=white)](https://learn.microsoft.com/powershell/)
[![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D6?logo=windows&logoColor=white)](https://www.microsoft.com/windows)
[![WinGet](https://img.shields.io/badge/WinGet-App%20Installer-0078D4?logo=windows&logoColor=white)](https://learn.microsoft.com/windows/package-manager/winget/)

## Funcionalidades
O script oferece um menu interativo com 10 opções principais e exibe informações importantes do sistema (SO, CPU, GPU, placa-mãe, RAM, disco e volume C) antes de executar as tarefas:

- Informações do sistema: exibe processador, placa-mãe, GPU, sistema operacional, RAM e disco.
- Reparo do sistema: executa DISM e SFC para corrigir arquivos do sistema corrompidos.
- Limpeza de temporários: libera espaço em disco removendo arquivos de cache do sistema e do usuário.
- Diagnóstico de rede: testa a comunicação com o gateway, DNS, google.com e a.ntp.br.
- Reset de rede: restaura os protocolos TCP/IP e limpa o cache de DNS para resolver problemas de conexão.
- Verificação de portas: valida se portas comuns de serviços estão abertas e acessíveis.
- Atualização de aplicativos: usa o Winget para atualizar todos os programas instalados de uma vez.
- Atualização de políticas: força a atualização das políticas de grupo locais com o comando gpupdate /force.
- Saúde do disco: lê dados S.M.A.R.T. para verificar se o HDD ou SSD está saudável.
- Reinício do spooler de impressão: reinicia o serviço do spooler de impressão para resolver problemas de impressão.
- Verificação de logs: analisa os logs gerados para identificar erros e auxiliar na solução de problemas.

## Requisitos
- Windows 10/11
- É necessário executar o script como Administrador, pois algumas ações exigem privilégios de sistema.

## Como executar
1. Acesse o repositório no GitHub.
2. Clique em Code e depois em Download ZIP.
3. Extraia o arquivo ZIP em uma pasta de sua preferência.
4. Entre na pasta extraída e execute o arquivo WinHealth.bat.
5. Se o Windows solicitar permissão, confirme para executar como Administrador.

> O script cria logs em uma pasta localizada em %PROGRAMDATA%\Logs_Manutencao