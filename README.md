# :thinking: Comandos para React-native

Comandos do react-native que salvam em qualquer hora que você estiver em desespero...

### Gerar apk:

```js
  cd android;gradlew clean;gradlew assembleRelease;cd ..
```

### Instalar dependencias no ios:

```js
yarn;cd ios;pod install; cd ..
```

### Instalar o aplicativo:

```js
cd android;./gradlew clean;cd ..;npx react-native run-android
```

### Limpar o gradlew:
```js
cd android;gradlew clean;cd ..
```

### Iniciar um projeto react-native TYPESCRIPT:
```js
npx react-native init apptest --template react-native-template-typescript
```

### Iniciar um projeto react-native JAVASCRIPT:
```js
npx react-native init apptest
```
### Instalando o ES-LINT:
```js
yarn add eslint -D 
```

### Iniciando o ES-LINT:
```js
yarn eslint --init
```

### Instalando o Prettier e seus plugins:
```js
yarn add prettier eslint-config-prettier eslint-plugin-prettier -D
```

### Instalando o config de import:
```js
yarn add eslint-import-resolver-typescript -D
```
### Instalando o React Navigation:
```js
yarn add @react-navigation/native
```

### Add no index ou App da raiz do projeto:
```js
import 'react-native-gesture-handler';
```
### Por volta de tudo deverá ter esse container:
```js
import { NavigationContainer } from '@react-navigation/native';

export default function App() {
  return (
    <NavigationContainer>{/* Rest of your app code */}</NavigationContainer>
  );
}
```



### Instalando o Stack Navigation:
```js
yarn add @react-navigation/stack
```

