<h1 align=center>Menu-gtk-python</h1>
<img width="1921" height="1081" alt="image" src="https://github.com/user-attachments/assets/9a1aa4bf-54cd-4258-9210-f97f8585aabf" />

<div align=center>
  
![Version](https://img.shields.io/badge/version-0.5.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-Em%20desenvolvimento-yellow.svg)

</div>

## Descrição

Um menu **construído** para o Linux que serve como interface do usuário para visualizar algumas informações e alterar outras, além de possuir um sistema de **tarefas** integrado.

## Tecnologias Utilizadas

- Python  
- GTK (framework)

## Dependências

São os pacotes necessários para o funcionamento esperado da aplicação.

Muitas das **dependências** referentes ao Linux podem ser ignoradas caso se deseje trocar as funcionalidades ou aplicativos/funções atrelados aos botões.

### 🐍 Python
As dependências Python podem ser instaladas via `pip`. É recomendado o uso de um ambiente virtual:
- **psutil**: Para monitoramento de CPU, RAM e sensores.
- **pydbus**: Para integração com o NetworkManager (Wi-Fi).
- **PyGObject**: Bindings para o GTK 4.
- **pycairo**: Motor de renderização 2D utilizado pelo GTK.

### 🐧 Sistema (Linux)
Certifique-se de ter o GTK 4 instalado e os seguintes utilitários para as funções dos botões:
- **GTK 4** (`libgtk-4-dev` ou `gtk4`)
- **GObject Introspection** (`libgirepository1.0-dev`)
- **brightnessctl**: Controle de brilho.
- **bluez**: Bluetooth (`bluetoothctl`).
- **swaync**: Centro de notificações.
- **wlogout**: Menu de logout.
- **power-profiles-daemon**: Perfis de energia.
- **pulseaudio-utils** ou **pipewire-pulse**: Controle de áudio (`pactl`).
- **hyprsunset**: Filtro de luz azul.
- **nvidia-utils**: Monitoramento de GPU (se usar NVIDIA).

---

## 🚀 Como Executar

Siga estes passos para configurar o ambiente e rodar a aplicação rapidamente:

### 1. Clonar o repositório
```bash
git clone https://github.com/Alberth-Farias/Menu-gtk-python.git
cd Menu-gtk-python
```

### 2. Criar um Ambiente Virtual (Venv)
Isso mantém as dependências do projeto isoladas do seu sistema.
```bash
python3 -m venv venv
```

### 3. Ativar o Ambiente Virtual
- **No Linux/macOS:**
```bash
source venv/bin/activate
```

### 4. Instalar as Dependências
```bash
pip install -r requirements.txt
```

> [!NOTE]
> Se a instalação do `PyGObject` falhar, certifique-se de ter os cabeçalhos de desenvolvimento do sistema instalados (ex: `sudo apt install libgirepository1.0-dev libcairo2-dev python3-dev`).

### 5. Executar a Aplicação
```bash
python3 main.py
```

