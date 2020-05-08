# :thinking: Comandos para React-native

Comandos do react-native que salvam em qualquer hora que você estiver em desespero...

### Gerar apk:

```js
  cd android && gradlew clean && gradlew assembleRelease && cd ..
```

### Instalar dependencias no ios:

```js
yarn && cd ios && pod install && cd ..
```

### Instalar o aplicativo:

```js
cd android && gradlew clean && cd .. && react-native run-android
```

### Limpar o gradlew:
```js
cd android && gradlew clean && cd ..
```
### Iniciar um projeto react-native:
```js
npx react-native init apptest --template react-native-template-typescript
```
