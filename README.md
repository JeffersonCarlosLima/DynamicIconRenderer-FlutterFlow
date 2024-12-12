# Dynamic Icon Renderer

**Dynamic Icon Renderer** é um widget Flutter que renderiza ícones dinamicamente com base no nome do ícone fornecido. Este componente permite personalização de cor, tamanho e dimensões, garantindo flexibilidade para atender diferentes designs e contextos de uso.

---

## Características principais
- Renderiza ícones dinamicamente com base no nome fornecido (`iconName`).
- Personalização de cor (`corIcone`) e tamanho (`tamanho`).
- Ajusta largura e altura do componente.

---

## Como usar

1. **Certifique-se de importar as bibliotecas necessárias** no seu projeto Flutter. Os seguintes imports são requeridos:

```dart
// Automatic FlutterFlow imports
import '/backend/schema/structs/index.dart';
import '/actions/actions.dart' as action_blocks;
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/custom_code/widgets/index.dart'; // Imports other custom widgets
import '/flutter_flow/custom_functions.dart'; // Imports custom functions
import 'package:flutter/material.dart';
```

2. **Adicione a classe `DynamicIconRenderer` ao seu projeto**:

```dart
class DynamicIconRenderer extends StatefulWidget {
  const DynamicIconRenderer({
    super.key,
    this.width,
    this.height,
    required this.iconName,
    this.corIcone = Colors.black,
    this.tamanho = 24.0,
  });

  final double? width;
  final double? height;
  final String iconName;
  final Color corIcone;
  final double tamanho;

  @override
  _DynamicIconRendererState createState() => _DynamicIconRendererState();
}
```

3. **Parâmetros do Widget**:
   - `width` *(opcional)*: Define a largura do widget.
   - `height` *(opcional)*: Define a altura do widget.
   - `iconName` *(obrigatório)*: Nome do ícone a ser renderizado.
   - `corIcone` *(opcional)*: Cor do ícone (padrão: `Colors.black`).
   - `tamanho` *(opcional)*: Tamanho do ícone (padrão: `24.0`).

---

## Exemplo de uso

```dart
DynamicIconRenderer(
  iconName: 'favorite',
  corIcone: Colors.red,
  tamanho: 32.0,
)
```

---

## Dependências necessárias
- **FlutterFlow**: Certifique-se de que o seu projeto usa o ambiente FlutterFlow para acessar os módulos como `flutter_flow_theme` e `flutter_flow_util`.
- **Widgets personalizados**: Garanta que o diretório `/custom_code/widgets/` existe e está configurado corretamente no seu projeto.

---

## Contribuições
Contribuições para o `Dynamic Icon Renderer` são bem-vindas! Sinta-se à vontade para abrir um _pull request_ ou relatar problemas na seção de _issues_.

---

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).
