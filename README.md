# nuxt-typescript


```
mkdir nuxt-typescript 
cd nuxt-typescript 
```

package.json作成
```
npm init -y
```
scriptのとこにdevを追加
```
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "nuxt"
  },
```
nuxtインストール
```
npm i --save nuxt
```

pagesディレクトリの作成
```
mkdir pages
```

pages/index.vueの作成して
```vue
<template>
    <h1>Hello world!</h1>
</template>
```

ts-node、@nuxt/typescriptをインストール
```
npm i -D ts-node @nuxt/typescript
```

ルートにnuxt.config.tsとtsconfig.jsonを作成

nuxt.config.ts
```typescript
import NuxtConfiguration from '@nuxt/config'

const config: NuxtConfiguration = {
};

module.exports = config
```

tsconfig.json
```json
{
  "compilerOptions": {
    "target": "es5",
    "module": "es2015",
    "moduleResolution": "node"
  }
}
```