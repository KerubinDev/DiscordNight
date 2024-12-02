![](https://i.imgur.com/XQApc9q.png)

Requer o aplicativo de desktop do [**Discord**](https://discordapp.com/) com [**BetterDiscord**](https://betterdiscord.app/) ou [**Vencord**](https://vencord.dev) instalado (ou qualquer outro mod de cliente Discord que suporte temas).

### [**BetterDiscord**](https://betterdiscord.app/):  
- Baixe o arquivo [**DiscordNight.theme.css**](https://betterdiscord.app/Download?id=155), acesse **Configurações > Temas** e clique em **Abrir Pasta de Temas**, ou coloque o arquivo em **%appdata%/BetterDiscord/themes** e ative o tema **DiscordNight**.  
Se o tema não aparecer, atualize o Discord usando **CTRL+R** ou reinicie o aplicativo.

### [**Vencord**](https://vencord.dev):  
- ***Método 1***:  
    - Baixe o arquivo [**DiscordNight.theme.css**](https://betterdiscord.app/Download?id=155), acesse **Configurações > Temas** e clique em **Abrir Pasta de Temas**, ou coloque o arquivo em **%appdata%/Vencord/themes** e ative o tema **DiscordNight**.  
- ***Método 2***:  
    - Vá em **Configurações > Temas**, acesse a aba **Temas Online**, e cole no campo de entrada o seguinte URL:  
```https://raw.githubusercontent.com/KillYoy/DiscordNight/master/DiscordNight.theme.css```

### Informações importantes

- O **Tema Escuro** precisa estar ativado em **Configurações > Aparência > Tema**, selecionando **Escuro**.
- As cores exclusivas para temas de usuários Nitro não são suportadas e podem apresentar falhas.

Tenha em mente que alterações podem ocorrer a qualquer momento devido a atualizações de fundo do Discord. Isso pode exigir a reinstalação do BetterDiscord ou aguardar a atualização do tema.  
Se houver algo que ainda não foi corrigido ou problemas relacionados a plugins, sinta-se à vontade para abrir uma nova [issue](https://github.com/KillYoy/DiscordNight/issues/new) ou entrar em contato comigo, **KillYoy#0295**, no Discord.

# Pré-visualização

Uma comparação com e sem o tema ativado no BetterDiscord (as imagens podem estar um pouco desatualizadas).

![Comparação da janela principal](https://i.imgur.com/fkQM8JW.png)  
Linhas sublinhadas correspondentes às funções da lista de membros requerem o plugin [**BetterRoleColors**](https://github.com/rauenzi/BetterDiscordAddons/tree/master/Plugins/BetterRoleColors).  
O tema suporta [**USRBG**](https://github.com/Discord-Custom-Covers/usrbg) criado por [**Tropical**](https://github.com/Tropix126).

![Comparação das configurações](https://i.imgur.com/5f6BjrR.png)

# Personalizando o tema

O DiscordNight possui variáveis exclusivas que podem ser modificadas facilmente para alterar a visibilidade e a largura de certos elementos. O código pode ser adicionado ao arquivo **DiscordNight.theme.css** ou no menu **CSS Personalizado** em Configurações do Discord:

```css
:root {
    --Channel-Invite-Edit-Buttons: none;                 /* flex = LIGADO, none = DESLIGADO */
    --Channel-Category-Invite-Button: flex;              /* flex = LIGADO, none = DESLIGADO */
    --Channel-List-Active-Threads: flex;                 /* flex = LIGADO, none = DESLIGADO */
    --Channel-List-Upcoming-Events: flex;                /* flex = LIGADO, none = DESLIGADO */
    --Channel-List-Boost-Goal: block;                    /* block = LIGADO, none = DESLIGADO */
    --Channel-List-Width: 200px;                         /* 200px, Padrão do Discord = 240px */
    
    --User-List-Width: 200px;                            /* 200px, Padrão do Discord = 240px */
    --User-Popout-Width: 240px;                          /* 240px, Padrão do Discord = 300px */
    --User-Status-Popout-Width: var(--User-Popout-Width);/* 240px, Padrão do Discord = 300px */
    
    --Search-List-Width: 488px;                          /* 488px, Padrão do Discord = 418px */
    --Inbox-List-Width: 522px;                           /* 522px, Padrão do Discord = 480px */
    
    --Emoji-Menu-Height: 618px;                          /* 618px ou 498px, Padrão do Discord = 444px */
    
    --Chatbox-Gift-Button: none;                         /* flex = LIGADO, none = DESLIGADO */
    --Chatbox-GIF-Button: none;                          /* flex = LIGADO, none = DESLIGADO */
    --Chatbox-Stickers-Button: none;                     /* flex = LIGADO, none = DESLIGADO */
    
    --Chat-Emoji-Size: 1.75rem;                          /* 1.75rem, Padrão do Discord = 1.375rem */
    --Chat-Emoji-Large-Size: 2rem;                       /* 2rem, Padrão do Discord = 3rem */
    --Chat-Sticker-Size: 5rem;                           /* 5rem, Padrão do Discord = 10rem */
    --Chat-Super-Reaction-Button: none;                  /* flex = LIGADO, none = DESLIGADO */
    --Chat-Wave-To-New-User-Button: flex;                /* flex = LIGADO, none = DESLIGADO */
    --Chat-Wave-To-New-DM-Button: flex;                  /* flex = LIGADO, none = DESLIGADO */
    
    --Text-Channels-Capital-Letter: capitalize;          /* capitalize, none */
    
    --Voice-Noise-Suppression: none;                     /* flex = LIGADO, none = DESLIGADO */
    --Start-Activities-Button: flex;                     /* flex = LIGADO, none = DESLIGADO */
    
    --Embed-Remove-Button: flex;                         /* flex = LIGADO, none = DESLIGADO */
    
    --Context-Menu-Emoji-Toolbar: none;                  /* flex = LIGADO, none = DESLIGADO */
    
    --Home-Nitro-Button: none;                           /* flex = LIGADO, none = DESLIGADO */
    --Home-Store-Button: none;                           /* flex = LIGADO, none = DESLIGADO */
    --Home-Direct-Messages-Header: flex;                 /* flex = LIGADO, none = DESLIGADO */
    --Home-Close-DM-Button: block;                       /* block = LIGADO, none = DESLIGADO */
    --Friends-List-Searchbar: none;                      /* flex = LIGADO, none = DESLIGADO */
    
    --Titlebar-Help-Icon: none;                          /* flex = LIGADO, none = DESLIGADO */
}
```

## Deseja que certos elementos permaneçam com a aparência padrão do Discord?
Eu criei alguns complementos que alteram certos aspectos do tema.  
Você pode alterar o **Aviso de Mensagens na Lista de Servidores** e o **Botão de Anexo no Chat** para voltarem à aparência original adicionando uma destas linhas de código ao arquivo **DiscordNight.theme.css**:

```css 
@import url("https://killyoy.github.io/DiscordNight/Addons/Vanilla_ServerList_Message_Notice.theme.css"); 
```   
```css 
@import url("https://killyoy.github.io/DiscordNight/Addons/Vanilla_Attachment_Button.theme.css"); 
```

# Instalando DiscordNight sem mods de cliente (não recomendado)

- Caso não queira usar BetterDiscord ou ele não funcione, o CSS pode ser injetado usando as ferramentas de desenvolvedor do Discord com **Ctrl+Shift+I** no aplicativo desktop ou **F12** no navegador. Na aba **Sources**, clique em **assets**, localize o arquivo que termina com **.css** e cole o código do **DiscordNight.css**. Se feito corretamente, o tema será carregado até que o Discord seja reiniciado (observe que imagens externas podem não ser carregadas dessa forma).

## Instalando DiscordNight no navegador

- Usando um complemento de estilos como o Stylus, você pode criar um estilo para **discordapp.com** e colar o código do **DiscordNight.css** (nem tudo funcionará corretamente, como barras de rolagem e imagens externas).
