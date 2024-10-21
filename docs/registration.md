# Components

## Registration

```ts
import { createApp } from 'ovee.js';
// Import component from library
import { YourComponent } from '@ovee.js/toolkit';

createApp()
    .compontent('your-component', YourComponent)
    .run(document.body);
```

## Registration with custom options

```ts
import { createApp } from 'ovee.js';
// Import component from library
import { YourComponent } from '@ovee.js/toolkit';

createApp()
    .compontent('your-component', YourComponent, {
        customField: 'custom'
    })
    .run(document.body);
```

## Registration multiple components

```ts
import { createApp } from 'ovee.js';
// Import component from library
import { YourComponent, MyComponent } from '@ovee.js/toolkit';

createApp()
    .compontents({
        'your-component': [YourComponent, {
            customField: 'custom'
        }],
        'my-component': [MyComponent]
    })
    .run(document.body);
```


## Styling

Some components have styles, which you can import in `SCSS`:

```scss
@import '@ovee.js/toolkit/styles/your-component';
```

# Modules

## Registration

```ts
import { createApp } from 'ovee.js';
// Import module from library
import { YourModule } from '@ovee.js/toolkit';

createApp()
    .use('your-module', YourModule)
    .run(document.body);
```

## Registration with custom options

```ts
import { createApp } from 'ovee.js';
// Import module from library
import { YourModule } from '@ovee.js/toolkit';

createApp()
    .use('your-module', YourModule, {
        customField: 'custom'
    })
    .run(document.body);
```

## Registration multiple modules

```ts
import { createApp } from 'ovee.js';
// Import module from library
import { YourModule, MyModule } from '@ovee.js/toolkit';

createApp()
    .useMany({
        'your-module': [YourModule, {
            customField: 'custom'
        }],
        MyModule: [MyModule]
    })
    .run(document.body);
```

## Styling

Some modules have styles, which you can import in `SCSS`:

```scss
@import '@ovee.js/toolkit/styles/your-module';
```