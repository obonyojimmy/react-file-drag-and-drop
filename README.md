# React File Drag and Drop Component
A simple React component that handles file drag and drop.

## How to use

```javascript
var FileDragAndDrop = require('react-file-drag-and-drop');

var Example = React.createClass({

  handleDrop: function (dataTransfer) {
    var files = dataTransfer.files;

    // Do something with dropped files...
  },

  render: function () {
    var style = {
      width: '100px',
      height: '100px'
    };

    return (
      <div>
        <h1>Please drop your files</h1>
        <div style={style}>
          <FileDragAndDrop onDrop={this.handleDrop} filesOnly={true}>

          </FileDragAndDrop>
        </div>
      </div>
    );
  }
});

module.exports = Example;
```
