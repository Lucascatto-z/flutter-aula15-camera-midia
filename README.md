# 📸 Perfil do Usuário — Câmera e Galeria de Mídia com Flutter

Aplicativo desenvolvido na disciplina de **Programação para Dispositivos Móveis I** (Aula 15). O projeto demonstra a integração com os recursos nativos de câmera fotográfica e galeria de fotos utilizando o pacote oficial `image_picker`[cite: 11].

---

## 🚀 Funcionalidades

* **Captura via Câmera Nativa:** Permite tirar fotos diretamente pelo aplicativo com ajuste automático de qualidade e largura máxima (`ImageSource.camera`)[cite: 11, 12].
* **Seleção da Galeria:** Abre o seletor nativo de imagens do dispositivo para escolher fotos armazenadas (`ImageSource.gallery`)[cite: 11, 12].
* **Interface Reativa de Perfil:** Exibe a imagem selecionada em uma moldura circular (`CircleAvatar` + `FileImage`), contando com avatar padrão quando nenhuma foto está definida e menu inferior (`showModalBottomSheet`) para escolha da origem[cite: 11, 12, 13, 14].

---

## 🛠️ Tecnologias Utilizadas

* **Flutter & Dart SDK**[cite: 11]
* **Pacote:** [`image_picker: ^1.1.0`](https://pub.dev/packages/image_picker)[cite: 11]
* **Manipulação de Arquivos:** `dart:io` (`File`)[cite: 11]

---

## 📁 Estrutura do Projeto

```text
lib/
├── screens/
│   └── perfil_screen.dart   # Interface gráfica do perfil e modal de mídia[cite: 12, 13]
├── services/
│   └── media_service.dart   # Camada de serviço encapsulando o ImagePicker[cite: 11, 12]
└── main.dart                # Ponto de entrada da aplicação[cite: 15]
