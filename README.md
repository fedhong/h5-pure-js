# h5-pure-js

### 纯JS实现H5页面开发的mini框架

### Hello world

```

import { createComponent, renderComponent } from 'h5-pure-js';

const tpl = '<div class="{{=it.style.name}}" onclick="onClickCb">Hello {{=it.data.name}}</div>'

const data = { name: 'Fedhong' };
const style = { name: 'bg' };
const events = {
    onClickCb: () => {

    }
}

const component = createComponent(tpl, { data, style }, events)

renderComponent(document.getElementById('app'), component)

```