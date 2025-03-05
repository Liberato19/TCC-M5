# Requisitos.

- M5 Cardputer
- Cartão SD

## 1 – Instalação.

### 1.1 - Preparação do cartão SD.

Formate o cartão SD em Fat32.

### 1.2 - Instalação do M5 Burner.

1. Acesse o site da M5Stack e procure pelo M5 Burner na aba de Softwares.
2. Faça o download do arquivo ZIP.
3. Execute o arquivo `M5Burner.exe`. Atualize o programa, se necessário.

![M5 Burner Installation](assets/Imagens/1.2.png)

### 1.3 – Instalação do M5Launcher.

1. Dentro do M5 Burner, selecione a aba **CARDPUTER**.
2. Localize e faça o download do firmware `M5Launcher.bin`.
3. Conecte o Cardputer ao computador e clique em **Burn**.
4. Selecione a porta COM referente ao dispositivo e clique em **Start**. Não desconecte o dispositivo durante o processo de Flash.

Se a instalação for bem-sucedida, o firmware estará pronto para uso.

![Burning Firmware](assets/Imagens/1.3.png)
![Burning Firmware Step 2](assets/Imagens/1.3(2).png)
![Burning Firmware Step 3](assets/Imagens/1.3.(3).png)

### 1.4 – Configurações no M5Launcher.

#### 1.4.1 - Verificação do cartão SD.

Na tela inicial, verifique se a opção **SD** está acessível. O ícone deve estar verde. Caso contrário, estará cinza.

![SD Card Verification](assets/Imagens/1.4.1.png)

#### 1.4.2 - Ativar modo Web Interface.

Selecione o ícone **WUI**. Você terá as seguintes opções:

- **My Network:** Conecte-se a uma rede Wi-Fi existente, fornecendo as credenciais.
- **AP Mode:** Inicie uma rede Wi-Fi aberta hospedada pelo Cardputer.

![Activating Web Interface](assets/Imagens/1.4.2.png)
![Activating Web Interface Step 2](assets/Imagens/1.4.2(2).png)
![Activating Web Interface Step 3](assets/Imagens/1.4.2(3).png)

Após escolher um método, o Cardputer exibirá um endereço IP que poderá ser acessado via navegador. Use as credenciais fornecidas pelo dispositivo para acessar a interface.

Na interface web, é possível gerenciar arquivos, monitorar o armazenamento e verificar a versão do firmware.

#### 1.4.3 - Download de Firmwares Secundários.

Para habilitar o multi-boot, adicione os firmwares necessários:

1. Acesse o repositório GitHub do **Evil-Cardputer**: [Evil M5Core2 Binaries](https://github.com/7h30th3r0n3/Evil-M5Core2/tree/main/binaries).
2. Alternativamente, use a interface web para baixar o firmware em **Online Firmware List**.
3. Faça o upload do arquivo `.bin` para o Cardputer via interface web.

![Downloading Secondary Firmware](assets/Imagens/1.4.3.png)
![Downloading Secondary Firmware Step 2](assets/Imagens/1.4.3(2).png)
![Downloading Secondary Firmware Step 3](assets/Imagens/1.4.3(3).png)

### 1.5 - Instalação do Evil-Cardputer.

1. Desative a interface web clicando em **OK**.
2. No menu inicial, selecione **SD** e localize o arquivo `.bin` enviado.
3. Escolha **Install** e aguarde a conclusão da instalação. O dispositivo será reiniciado automaticamente.

![Installing Evil-Cardputer](assets/Imagens/1.5.png)
![Installing Evil-Cardputer Step 2](assets/Imagens/1.5(2).png)
![Installing Evil-Cardputer Step 3](assets/Imagens/1.5(3).png)

O Cardputer está configurado e pronto para uso!

## 2 - Guia de Uso.
Siga estas etapas para utilizar com eficiência cada recurso do Evil-Cardputer, neste guia vamos apenas abordar as funções que sejam relacionadas ao tema, para mais informações acesse o [guia oficial do firmware](https://github.com/7h30th3r0n3/Evil-M5Project/blob/main/README.md).

### 2.1 - Menu.

- Menu Principal do firmware
  
![Menu](assets/Imagens/2.1.png)

#### 2.2 - Scan WiFi.

- Realiza um scan a procura de WiFis próximos.

#### 2.3 - Select Network.

- Escolhe uma rede WiFi da lista de WiFis escaneados , utilize as teclas de direita e esquerda para navegar no menu.
  
![Select Network](assets/Imagens/2.2.png)

#### 2.4 - Clone & Details.

- Informações sobre a rede escolhida, você pode clonar o SSID neste menu.
  
![Clone & Details](assets/Imagens/2.3.png)

#### 2.5 - Set WiFi SSID.

- Configure o SSID da rede a ser criada.

#### 2.6 - Set WiFi Password.

- Configure a senha da rede a ser criada.


#### 2.7 - Set WiFi Mac Adress.

- Configure o endereço MAC da rede a ser criada.

#### 2.8 - Start Captive Portal.

- Utilizando o `normal.html`, inicia uma rede de wifi e imita uma tela de login junto de uma tela de erro.

![Clone & Details](assets/Imagens/2.8.png)
![Clone & Details](assets/Imagens/2.8(1).png)
![Clone & Details](assets/Imagens/2.8(2).png)

#### 2.7 - Stop Captive Portal.

- Desativa o Captive Portal e DNS.

#### 2.8 - Change Portal.

- Troca a página HTML do Captive Portal por uma armazenada no cartão SD.

#### 2.8 - Change Portal.

- Troca a página HTML do Captive Portal por uma armazenada no cartão SD.

#### 2.9 - Check Credentials.

- Lista as credenciais adquiridas com a pagina de login falsa.

#### 2.10 - Delet All Creds.

- Apaga as credenciais adquiridas.

#### 2.10 - Monitor Status.

- Monitora o status do Captive Portal como número de clientes conectados, SSID e IP e número de credenciais adquiridas.

#### 2.11 - Probe Attack.

- Envia Probe Requests falsas e aleatórias em todos os canais

#### 2.12 - Probe Sniffing.

- Probe Sniffing inivia um probe scan que captura os SSID recebidos que podem ser armazenados e reutilizados. Limite de 150 probes.

#### 2.13 - Karma Attack.

- Semelhante ao Probe Sniffing, mas exibe um menu após a finalização da varredura para escolher um SSID específico. Quando um SSID é selecionado, um portal com o mesmo SSID é implantado. Se o ponto de acesso original for uma Rede Aberta e a máquina for vulnerável, ela deve se conectar automaticamente à rede. Dependendo da máquina, o portal pode ser exibido automaticamente.
Se um cliente estiver presente no momento em que a varredura termina ou é interrompida, o portal permanece aberto; caso contrário, ele é desligado. (Pode ser usado com senha se configurado na interface web).

#### 2.14 - Karma Attack.

- Semelhante ao Karma Attack, mas tenta automaticamente a primeira probe detectada. Se nenhum cliente se conectar após 15 segundos, o Cardputer retorna ao modo de sniffing para tentar outra probe capturada, continuando esse ciclo até que o usuário interrompa o processo.
Também pode ser usado com senha se configurado na interface web. Se você tiver uma senha, mas não souber em qual AP ela funciona, pode testá-la com diferentes probe requests para verificar se o Karma funciona e obter o SSID.
Essa funcionalidade é inspirada no projeto Pwnagotchi, mas combinando probe request e karma attack, permitindo um ataque completo aos dispositivos próximos.
Você pode adicionar SSIDs à KarmaAutoWhitelist da seguinte forma:
KarmaAutoWhitelist=notmybox,thisonetoo
As probes dessas redes serão ignoradas e uma mensagem será enviada via serial notificando que a rede está na lista de permissões. Isso também funciona no Probe Sniffing e no Karma Attack.

#### 2.15 - Karma Spear.

- Semelhante ao Karma Auto, mas usa SSIDs abertos capturados por wardriving. Você também pode adicionar SSIDs personalizados ao arquivo KarmaList.txt.

#### 2.16 - Selecionar Probe.

- Menu para selecionar um SSID de probe capturado anteriormente e implantá-lo. A lista é limitada a 150 probes.

#### 2.17 - Deletar Probe.

- Menu para excluir um SSID de probe capturado anteriormente. A lista é limitada a 150 probes.

#### 2.18 - Deletar Todas as Probes.

- Exclui todas as probes capturadas anteriormente. Basicamente, redefine o arquivo probes.txt no SD.

#### 2.19 - Wardriving.

- Escaneia redes Wi-Fi ao redor e as vincula à posição no formato Wigle. Você pode fazer upload para o Wigle para ganhar pontos e gerar um arquivo KML para visualização no Google Earth. É necessário um módulo GPS para essa funcionalidade.

#### 2.20 - Beacon Spam.

- O Beacon Spam cria múltiplas redes em todos os canais, exibindo vários SSIDs na busca Wi-Fi e confundindo equipamentos de sniffing. Você pode utilizar Beacons personalizados por meio de um arquivo de configuração.

#### 2.21 - Client Sniff e Deauth

- Na Tela:
    AP: Número de APs próximos
    C: Canal atual
    H: Número de novos arquivos PCAP criados (contendo pelo menos um EAPOL e um beacon frame)
    E: Número de pacotes EAPOL capturados
    D: 0 = apenas sniffing, sem deauth / 1 = deauth ativo
    DF: Modo Rápido
O que ele faz:
    Escaneia APs próximos
    Detecta se um cliente está conectado
    Envia frames de deautenticação em broadcast para cada AP com clientes conectados
    Envia frames de deauth spoofed para cada cliente
    Sniffa pacotes EAPOL ao mesmo tempo
    Retorna ao escaneamento de APs próximos
  
#### 2.22 - Deauther

- Envia frames de deautenticação e sniffa pacotes EAPOL ao mesmo tempo.
    Selecione a rede alvo
    Vá para Deauther
    Responda às perguntas solicitadas
    Inicie o ataque de deauth e sniff simultaneamente

#### 2.23 - EAPOL Sniffing

- Captura pacotes EAPOL (4-way handshake e PMKID)
Parâmetros:
    Canal: Canal atual
    Modo:
        Estático → Fica no mesmo canal
        Automático → Alterna entre os canais
    PPS: Pacotes por segundo no canal (se não houver atividade, o valor pode ficar travado até que um novo pacote seja recebido)
    H: Número de novos PCAPs criados (mínimo um EAPOL e um beacon frame)
    EAPOL: Número de pacotes EAPOL capturados
    DEAUTH: Número de pacotes Deauth detectados
    RSSI: Potência do sinal (indica a distância do transmissor)

Se um pacote EAPOL for detectado, ele é armazenado em um arquivo PCAP, junto com o MAC do AP e beacon frames com o BSSID. Você pode usar ferramentas como Aircrack-ng ou Hashcat para quebrar a senha da rede Wi-Fi a partir de um 4-way handshake ou PMKID.
Detecta pacotes de deautenticação próximos, quando um dispositivo se desconecta de um AP ele envia um pacote de deautenticação para encerrar a conexão. Esses pacotes podem ser falsificados por atacantes para desconectar dispositivos e forçá-los a se reconectar, permitindo a captura do 4-way handshake. Um grande número de pacotes de deauth não é normal e pode indicar um possível ataque Wi-Fi.






