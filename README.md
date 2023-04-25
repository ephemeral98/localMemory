## 使用方法：

### 方法
1. localMemory (使用的是localStorage)
2. sessionMemory (使用的是sessionStorage)

### 设置
```js
import { localMemory } from 'localmemory';
localMemory.setItem({ name: 'account', value: 'barry' });
```

设置两天后过期：
```js
// 设置两天后登录过期
localMemory.setItem({ name: 'account', value: 'barry', expired: 3600 * 24 * 2 });
```

### 获取
```js
import { localMemory } from 'localmemory';
localMemory.getItem('account')
```
