<img src='https://cloud.githubusercontent.com/assets/29597/12027069/779d8f3c-ad8f-11e5-8bac-2f6e8eed7192.png' width='250' height='123' alt='redux devtools filterable log monitor logo'/>
=========================

Filterable tree view monitor for [Redux DevTools](https://github.com/gaearon/redux-devtools).
Check out a [simple demo application here](https://bvaughn.github.io/redux-devtools-filterable-log-monitor).

<img width='624' height='448' alt='Demo GIF' src='https://cloud.githubusercontent.com/assets/29597/12024861/a510cb96-ad76-11e5-9ce3-78f46a2f6837.gif'/>

Installation
------------

```
npm install --save-dev redux-devtools-filterable-log-monitor
```

Usage
------------

The `FilterableLogMonitor` is intended for use within the [`DockMonitor`](https://github.com/gaearon/redux-devtools-dock-monitor). You can configure your app to use these monitors like so:

```js
import React from 'react'
import { createDevTools } from 'redux-devtools'
import DockMonitor from 'redux-devtools-dock-monitor'
import FilterableLogMonitor from '../src'

const DevTools = createDevTools(
  <DockMonitor toggleVisibilityKey='ctrl-h'
               changePositionKey='ctrl-q'>
    <FilterableLogMonitor/>
  </DockMonitor>
)

export default DevTools

```

Then you can render `<DevTools>` to any place inside app or even into a separate popup window.

[Read how to start using Redux DevTools.](https://github.com/gaearon/redux-devtools)

Features
------------

Every action is displayed in the log. Use the filter input to quickly and easily locate nodes in your store that are deeply nested. You can search using regular expressions or simple strings. Select whether the search should match keys, values, or either using the checkboxes above the filter input.

Contributions
------------

Use [GitHub issues](https://github.com/bvaughn/redux-devtools-filterable-log-monitor/issues) for requests.

I actively welcome pull requests; learn how to [contribute](https://github.com/bvaughn/react-virtualized/blob/master/CONTRIBUTING.md).

Changelog
---------

Changes are tracked in the [changelog](https://github.com/bvaughn/redux-devtools-filterable-log-monitor/blob/master/CHANGELOG.md).

License
---------

*react-virtualized* is available under the MIT License.
