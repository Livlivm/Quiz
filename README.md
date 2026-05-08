#  Quiz Flutter

Projeto desenvolvido em Flutter como atividade final da aula.  
O aplicativo funciona como um quiz interativo com perguntas carregadas através de um arquivo JSON.

---

##  Funcionalidades

- Splash Screen animada
- Perguntas com alternativas
- Resposta na hora 
- Uso de imagens externas
- Geração de APK Android

---

## Tecnologias Utilizadas

- Flutter
- Dart
- JSON
- Material Design

---

##  Perguntas em JSON

Arquivo utilizado:

```bash
assets/mokup/perguntas.json
```

Modelo:

```json
[
  {
    "id": 1,
    "ilustracao":"https://admin.cnnbrasil.com.br/wp-content/uploads/sites/12/2021/06/26776_1798DEE935286D54.jpg?w=1024",
    "pergunta": "Qual o primeiro computador digital construído?",
    "respostas": [
      "Robotinic",
      "ENIAC",
      "ABACO",
      "Máquina de calcular de Leibniz"
    ],
    "correta": 2
  }
]
```

---

##  Configuração do pubspec.yaml

```yaml
dependencies:
  flutter:
    sdk: flutter

dev_dependencies:
  flutter_test:
    sdk: flutter

  flutter_lints: ^6.0.0
  flutter_launcher_icons: ^0.14.1

flutter:

  uses-material-design: true

  assets:
    - assets/mokup/perguntas.json
    - assets/icone.png

flutter_launcher_icons:
  android: true
  ios: true
  image_path: "assets/icone.png"
  remove_alpha_ios: true
```

---

## Executando o Projeto

Instalar dependências:

```bash
flutter pub get
```

Executar:

```bash
flutter run
```

Executar no Chrome:

```bash
flutter run -d chrome
```

---

##  Alterando Ícone

```bash
dart run flutter_launcher_icons
```

---


##  Enviando para GitHub

```bash
git init
git add .
git commit -m "Projeto Quiz Flutter"
git remote add origin LINK_DO_REPOSITORIO
git push -u origin main
```

---

## Desenvolvido por
Livia Morais Pereira 
