# :thinking: Comandos que salvam

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

### Instalar e rodar um app react-native no Ubuntu-Linux

```js
  yarn android;yarn start
```

##### Este comando é devido o bundle não abrir, neste caso teremos que rodar o bundle em um terminal.

### Limpar o gradlew:
```js
cd android;gradlew clean;cd ..
```

### Trabalhar localmente utilizando API, para que o emulador consiga acessar:

```js
adb reverse tcp:9090 tcp:9090
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

### Postgres no ubuntu
```js
sudo -u postgres psql
```

### Escolher client no dbeaver (ubuntu):

```
/usr/bin/pg_dump
```
### Restore database per line of code (ubuntu):

```
sudo -u postgres psql -U postgres -d database < '/caminho-da-image'
```
É necessario ter o postgresSQL instalado localmente em sua maquina

### Erro ao dar yarn muitas vezes:

```
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p'
```
#### React error: Import in body of module; reorder to top

```
adicione na frente da linha que está o erro este comando comentado: // eslint-disable-line
```

#### Desabiliar eslint:
```
To disable all rules on a specific line, use a line comment in one of the following formats: alert('foo'); // eslint-disable-line // eslint-disable-next-line alert('foo'); To disable a specific rule on a specific line: alert('foo'); // eslint-disable-line no-alert // eslint-disable-next-line no-alert alert('foo');
```

#### install golang ubuntu:

```` 
sudo apt install golang-go
````

