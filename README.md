Bare Bones Project using dsimard/grunt-angular-phonegap

## Usage

1. Clone project

2. Install npm modules

        npm install

3. Install bower dependencies

        bower install

4. Add a mobile platform

        cordova platform add android

4. Build the project

        grunt phonegap:build

5. Deploy to device

        cordova use android *or* grunt phonegap:emulate for emulation

6. Send the project to remotely build at http://build.phonegap.com.

```
phonegap remote login --username you@gmail.com --password YourPassword
grunt phonegap:send
```

### Step 1

[Create project](https://github.com/rhalff/robberthalff-app/commit/f3ff34470e927a723f468e4300d1f075eb22724e)
```
cordova create robberthalff-app
```

[Add Android Target](https://github.com/rhalff/robberthalff-app/commit/22d89466dfdbfcdf64c3f13bc64e1526776af930)
```
cordova platform add android
```

[Yo Angular](https://github.com/rhalff/robberthalff-app/commit/cd3147cf5b045a61255bbcc620bab7dc0da8d9e1)
```
yo angular robberthalff
```

Add [grunt-angular-phonegap](https://github.com/dsimard/grunt-angular-phonegap)
```
npm install grunt-angular-phonegap --save-dev
```

[Build it!](https://github.com/rhalff/robberthalff-app/commit/ed3298b5d5945026256f6aa18b5fe74d786dea8c)
```
grunt phonegap:build
cordova run android
```

Add dependencies for karma (Not automatically installed by yo angular)
```
npm install karma-chrome-launcher --save-dev
npm install karma-jasmine --save-dev
```

Docs:

  - yeoman angular: https://github.com/yeoman/generator-angular
  - Karma: http://karma-runner.github.io/0.12/index.html
