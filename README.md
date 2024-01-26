# :thinking: Comandos que salvam

Comandos que salvam em qualquer hora que você estiver em desespero...

### Gerar apk:

```js
  cd android;gradlew clean;gradlew assembleRelease;cd ..
```

### Instalar dependencias no ios:

```js
yarn;cd ios;pod install; cd ..
```

### Instalar o aplicativo android:

```js
cd android;./gradlew clean;cd ..;npx react-native run-android

ou

cd android;./gradlew clean;cd ..;yarn android

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

### Initial app expo typescript
````js
expo init --template expo-template-bare-typescript --name appname
````


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
To disable all rules on a specific line, use a line comment in one of the following formats: alert('foo'); 
// eslint-disable-line;
// eslint-disable-next-line alert('foo'); To disable a specific rule on a specific line: alert('foo'); 
// eslint-disable-line no-alert;
// eslint-disable-next-line no-alert alert('foo');
```

#### install golang ubuntu:

```` 
sudo apt install golang-go
````

#### install brew ubuntu:

```` 
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
````

#### Iniciar um projeto com NextJS:

````
yarn create next-app nomeprojeto
````

#### Depois para utilizar typescript rode o comando:
````
yarn add typescrpt @types/node @types/react -D
````

#### Padrão da Data pt-BR:

````js

  const options = { year: "numeric", month: "long", day: "numeric" };
  const date = new Date(2020, 11, 31) // 2020-12-31T03:00:00.000Z
  console.log(date.toLocaleDateString("pt-br", options))
  // 31 de dezembro de 2020
  console.log(date.toLocaleDateString("pt-br", { ...options, month: 'numeric'}))
  // 31/12/2020

  const regex = /^([0-9]{4})[-](0[1-9]|1[0-2])[-](0[0-9]|1[0-9]|2[0-9]|3[0-1])/gm
  const dateRx = new Date(2020, 11, 31) // 2020-12-31T03:00:00.000Z
  const [full, year, month, day] = regex.exec(dateRx.toISOString())

  console.log(`${day}/${month}/${year}`)
  // 31/12/2020
````

### Mascara de input para R$:

````
export function maskCurrency(value: string): string {
  return value
    .replace(/\D/g, '')
    .replace(/(\d)(\d{2})$/, '$1,$2')
    .replace(/(?=(\d{3})+(\D))\B/g, '.');
}
````
### utilizando sequelize:

````
npm install --save-dev sequelize-cli

npx sequelize-cli init
````

### setando variaveis de ambinet no windows (ex. Android Studio):

````
setX /M ANDROID_HOME "C:\Users\pdjkl\AppData\Local\Android\Sdk"
setX /M PATH "%ANDROID_HOME%\tools;%PATH%"
setX /M PATH "%ANDROID_HOME%\platform-tools;%PATH%"
````

### Projetos que não utilizam yarn para instalar de forma melhor as dependencias utilize:

````
npm ci --silent
````

### Default branch main:

````
git config --global init.defaultBranch main
````

### Criar projeto flutter com linha de comando:

````
flutter create testeapp
````

### Inicializando seu projeto flutter
````
cd testeapp
flutter run
````

### Install mysql and mysqlWorkbench:
````
sudo apt update
sudo apt upgrade
sudo apt-get install mysql-server mysql-client (isso não é para docker)
sudo apt install mysql-workbench
````
### Kill process in port 3000
````
sudo lsof -i:3000
sudo kill PID
````

### Flutter get packages
````
flutter pub get
````

### Merge abort
````
git merge --abort
````

## git merge 
````
git merge --no-ff nome_da_branch
````
## git fetch 
````
git fetch
````

## install Vagrant 
````
curl -O https://releases.hashicorp.com/vagrant/2.2.9/vagrant_2.2.9_x86_64.deb
sudo apt install ./vagrant_2.2.9_x86_64.deb

teste:
vagrant --version

vagrant plugin install vagrant-disksize

vagrant plugin install vagrant-vbguest
````
## Error: ENOSPC: System limit for number of file watchers reached:

````
cat /proc/sys/fs/inotify/max_user_watches -> retorna 8192;

echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p -> para ajustar o limite novo
````

## Delete branch in Git

````
git branch -d 'nome da sua branch'
````

## Initialize vagrant and signIn vagrant

````
vagrant up;vagrant ssh
````


## Install Postgress ubuntu 18.04

````
sudo apt update
sudo apt install postgresql postgresql-contrib
````

### Dar premissão a um diretório

````
sudo chmod -R 777 diretorio
````

### Comands config VPN

````
openvpn --config /etc/openvpn/arquivo-de-config.opvn
````

flutter run --no-sound-null-safety
<br/>
yarn prisma db pull

````
git push --delete origin 0.0.0
git tag -l
git push -f
````


````
git submodule status
git submodule init
git submodule update
````

Regex orders vtex
````
/^[\d\w-]{5,20}$/
````
