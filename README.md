# bpmn-js collapse subprocess

A bpmn-js extension that re-enables to collapse sub process via replace menu. This package **does not** introduce any changes for plain bpmn-js. Its only purpose is to be able to reverse changes introduced via [bpmn-js-disable-collapsed-subprocess](https://github.com/bpmn-io/bpmn-js-disable-collapsed-subprocess), if you need to.

## Installation

Install via [npm](http://npmjs.com/).

```bash
npm install bpmn-js-collapse-subprocess
```

Add as additional module to [bpmn-js](https://github.com/bpmn-io/bpmn-js).

### Modeler

```javascript
var BpmnModeler = require('bpmn-js/lib/Modeler');
var disableCollapsedSubprocessModule = require('bpmn-js-disable-collapsed-subprocess');
var collapseSubprocessModule = require('bpmn-js-collapse-subprocess');

var modeler = new BpmnModeler({
  container: '#canvas',
  additionalModules: [
    disableCollapsedSubprocessModule,
    collapseSubprocessModule
  ]
});
```

### Viewer

This extension is useless for the Viewer as it changes modeling actions.

## Licence

MIT
