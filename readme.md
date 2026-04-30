# @ctrlo/filedrag

Simple drag and drop JQuery plugin

## Usage

```javascript
const options = {
    allowMultiple: true, //optional, defaults to true
    debug: false // optional, defaults to false
};

$element.filedrag(options);

/*
Triggered when a file is dropped on the control
event has signature {
    file: File,
    index: number,
    length: number
}
*/
$element.on('fileDrop', (ev)=>{
    console.log(ev)
});

//Triggered when all files have been uploaded
$element.on('uploadsComplete', (ev)=>{
    console.log('Complete');
});
```