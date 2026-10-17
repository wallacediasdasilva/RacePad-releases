<p align="center"><img src="racepad-icon.svg" width="140" alt="RacePad"></p>

# RacePad

Transforma o celular Android em uma **button box de cockpit** para jogos de simulação no PC
(corrida, caminhão...). Cada botão do celular aperta uma tecla no Windows pela rede Wi‑Fi de casa.

- Botões redondos, interruptores de alavanca e interruptor com capa (ignição), com ícones
- Painel livre: mova, redimensione, adicione e remova controles; desfazer/refazer
- Perfis por jogo (modelos prontos de Corrida e Caminhão), retrato e paisagem em tela cheia
- Teclas F13–F24 por padrão: não conflitam com nenhum atalho e os jogos aceitam no mapeamento

## Download

Baixe a versão mais recente em **[Releases](../../releases/latest)**:

| Arquivo | Para |
|---|---|
| `RacePad-Setup-x.y.z.exe` | PC com Windows 10 ou 11 (64 bits) |
| `RacePad-x.y.z.apk` | celular Android 7.0 ou mais novo |

## Instalação

### 1. No PC

1. Rode `RacePad-Setup-x.y.z.exe`.
   O Windows pode mostrar **"O Windows protegeu o computador"** (o instalador não tem assinatura digital
   paga): clique em **Mais informações → Executar assim mesmo**.
2. Deixe marcadas as opções **Liberar no Firewall** e **Iniciar junto com o Windows**.
3. O RacePad Receiver fica como ícone na bandeja, perto do relógio. Clique com o botão direito para ver o
   IP do PC.

A rede Wi‑Fi de casa precisa estar como **Rede privada** no Windows
(Configurações → Rede e Internet → sua rede → Rede privada).

### 2. No celular

1. Baixe o `RacePad-x.y.z.apk` no celular e abra.
2. O Android vai pedir para **permitir instalar apps desta fonte** (navegador ou gerenciador de
   arquivos): permita e confirme a instalação.

### 3. Conectar

1. Celular e PC na **mesma rede Wi‑Fi**.
2. No app: **Config → Procurar na rede → Salvar**.
3. Toque num botão: o status embaixo mostra a tecla enviada.

### 4. No jogo

Nas configurações de controles do jogo, escolha a ação (ex.: "Ligar motor") e toque o botão
correspondente no celular para o jogo gravar a tecla.

## Problemas comuns

- **O celular não encontra o PC:** confira se o RacePad Receiver está na bandeja, se a rede do Windows
  está como Privada e se os dois estão no mesmo Wi‑Fi (redes de convidados costumam isolar aparelhos).
- **A tecla chega no PC mas não no jogo:** se o jogo roda como administrador, abra o RacePad Receiver como
  administrador também (botão direito → Executar como administrador).

## Conferir os downloads

Cada release traz `SHA256SUMS.txt`. No PowerShell: `Get-FileHash .\RacePad-Setup-x.y.z.exe`
e compare com o valor do arquivo.

## Desinstalar

- PC: Configurações → Aplicativos → **RacePad** → Desinstalar (remove também a regra do Firewall e o
  início automático).
- Celular: como qualquer app.