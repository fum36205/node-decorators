![Node Decorators](https://github.com/serhiisol/node-decorators/blob/master/decorators.png?raw=true)

### Common Decorators

### Installation
```
npm install @decorators/common --save
```
### API
#### Decorators
##### Method
* @Debounce(wait: number = 500) - postpone its execution until after wait milliseconds have elapsed since the last time it was invoked
* @Throttle(wait: number = 500) - when invoked repeatedly, will only actually call the original function at most once per every wait milliseconds 

```typescript
import { Debounce, Throttle } from '@decorators/common';

class TestController {
  @Debounce()
  debouncedAction() {
    console.log('debouncedAction');
  }
  
  @Throttle()
  throttledAction() {
    console.log('throttledAction');
  }
}
```

### License
MIT

[CoJS]:https://github.com/tj/co
