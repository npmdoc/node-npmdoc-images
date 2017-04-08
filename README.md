# api documentation for  [images (v3.0.0)](https://github.com/zhangyuanwei/node-images#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-images.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-images) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-images.svg)](https://travis-ci.org/npmdoc/node-npmdoc-images)
#### Cross-platform image decoder(png/jpeg/gif) and encoder(png/jpeg) for Node.js

[![NPM](https://nodei.co/npm/images.png?downloads=true)](https://www.npmjs.com/package/images)

[![apidoc](https://npmdoc.github.io/node-npmdoc-images/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-images%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-images/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-images/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-images/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "ZhangYuanwei",
        "email": "zhangyuanwei1988@gmail.com"
    },
    "bindingMap": {
        "0.8.0": [
            "0.8.0",
            "0.8.25"
        ],
        "0.9.11": [
            "0.10.0",
            "0.10.99"
        ],
        "0.12.0": [
            "0.12.0",
            "0.12.99"
        ],
        "4.0.0": [
            "4.0.0",
            "4.99.99"
        ],
        "5.0.0": [
            "5.0.0",
            "5.99.99"
        ],
        "6.0.0": [
            "6.0.0",
            "6.99.99"
        ]
    },
    "bindingsCDN": "https://raw.githubusercontent.com/zhangyuanwei/node-images/master/bindings/",
    "bugs": {
        "url": "https://github.com/zhangyuanwei/node-images/issues"
    },
    "dependencies": {
        "nan": "^2.3.2"
    },
    "description": "Cross-platform image decoder(png/jpeg/gif) and encoder(png/jpeg) for Node.js",
    "devDependencies": {
        "step": "0.0.5"
    },
    "directories": {},
    "dist": {
        "shasum": "e1c3866b7884d671a581fedd511134620da86ea1",
        "tarball": "https://registry.npmjs.org/images/-/images-3.0.0.tgz"
    },
    "gitHead": "094470e68bdc0744d38b413322d5a0e098347a37",
    "gypfile": true,
    "homepage": "https://github.com/zhangyuanwei/node-images#readme",
    "keywords": [
        "image",
        "decoder",
        "encoder",
        "png",
        "jpeg",
        "gif",
        "cross-platform",
        "images"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "2betop",
            "email": "2betop.cn@gmail.com"
        },
        {
            "name": "fansekey",
            "email": "fansekey@gmail.com"
        },
        {
            "name": "fis-dev",
            "email": "fansekey@gmail.com"
        },
        {
            "name": "zhangyuanwei",
            "email": "zhangyuanwei1988@gmail.com"
        }
    ],
    "name": "images",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/zhangyuanwei/node-images.git"
    },
    "scripts": {
        "install": "echo \"Hello, World.\"",
        "test": "node test.js"
    },
    "version": "3.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module images](#apidoc.module.images)
1.  [function <span class="apidocSignatureSpan">images.</span>Image (width, height)](#apidoc.element.images.Image)
1.  [function <span class="apidocSignatureSpan">images.</span>copyFromImage (src, x, y, width, height)](#apidoc.element.images.copyFromImage)
1.  [function <span class="apidocSignatureSpan">images.</span>createImage (width, height)](#apidoc.element.images.createImage)
1.  [function <span class="apidocSignatureSpan">images.</span>gc ()](#apidoc.element.images.gc)
1.  [function <span class="apidocSignatureSpan">images.</span>getUsedMemory ()](#apidoc.element.images.getUsedMemory)
1.  [function <span class="apidocSignatureSpan">images.</span>loadFromBuffer (buffer, start, end)](#apidoc.element.images.loadFromBuffer)
1.  [function <span class="apidocSignatureSpan">images.</span>loadFromFile (file)](#apidoc.element.images.loadFromFile)
1.  [function <span class="apidocSignatureSpan">images.</span>setGCThreshold (value)](#apidoc.element.images.setGCThreshold)
1.  [function <span class="apidocSignatureSpan">images.</span>setLimit (maxWidth, maxHeight)](#apidoc.element.images.setLimit)
1.  number <span class="apidocSignatureSpan">images.</span>TYPE_BMP
1.  number <span class="apidocSignatureSpan">images.</span>TYPE_GIF
1.  number <span class="apidocSignatureSpan">images.</span>TYPE_JPEG
1.  number <span class="apidocSignatureSpan">images.</span>TYPE_PNG
1.  number <span class="apidocSignatureSpan">images.</span>TYPE_RAW
1.  object <span class="apidocSignatureSpan">images.</span>Image.prototype
1.  object <span class="apidocSignatureSpan">images.</span>binding

#### [module images.Image](#apidoc.module.images.Image)
1.  [function <span class="apidocSignatureSpan">images.</span>Image (width, height)](#apidoc.element.images.Image.Image)

#### [module images.Image.prototype](#apidoc.module.images.Image.prototype)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>copyFromImage ()](#apidoc.element.images.Image.prototype.copyFromImage)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>draw ()](#apidoc.element.images.Image.prototype.draw)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>drawImage ()](#apidoc.element.images.Image.prototype.drawImage)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>encode ()](#apidoc.element.images.Image.prototype.encode)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>fill ()](#apidoc.element.images.Image.prototype.fill)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>fillColor ()](#apidoc.element.images.Image.prototype.fillColor)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>height ()](#apidoc.element.images.Image.prototype.height)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>loadFromBuffer ()](#apidoc.element.images.Image.prototype.loadFromBuffer)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>resize ()](#apidoc.element.images.Image.prototype.resize)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>save ()](#apidoc.element.images.Image.prototype.save)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>saveAsync ()](#apidoc.element.images.Image.prototype.saveAsync)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>size ()](#apidoc.element.images.Image.prototype.size)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>toBuffer ()](#apidoc.element.images.Image.prototype.toBuffer)
1.  [function <span class="apidocSignatureSpan">images.Image.prototype.</span>width ()](#apidoc.element.images.Image.prototype.width)

#### [module images.binding](#apidoc.module.images.binding)
1.  [function <span class="apidocSignatureSpan">images.binding.</span>Image ()](#apidoc.element.images.binding.Image)
1.  [function <span class="apidocSignatureSpan">images.binding.</span>gc ()](#apidoc.element.images.binding.gc)
1.  number <span class="apidocSignatureSpan">images.binding.</span>TYPE_BMP
1.  number <span class="apidocSignatureSpan">images.binding.</span>TYPE_GIF
1.  number <span class="apidocSignatureSpan">images.binding.</span>TYPE_JPEG
1.  number <span class="apidocSignatureSpan">images.binding.</span>TYPE_PNG
1.  number <span class="apidocSignatureSpan">images.binding.</span>TYPE_RAW
1.  number <span class="apidocSignatureSpan">images.binding.</span>maxHeight
1.  number <span class="apidocSignatureSpan">images.binding.</span>maxWidth
1.  number <span class="apidocSignatureSpan">images.binding.</span>usedMemory



# <a name="apidoc.module.images"></a>[module images](#apidoc.module.images)

#### <a name="apidoc.element.images.Image"></a>[function <span class="apidocSignatureSpan">images.</span>Image (width, height)](#apidoc.element.images.Image)
- description and source-code
```javascript
function WrappedImage(width, height) {
    if (!(this instanceof WrappedImage)) return new WrappedImage(width, height);
    if (gcThreshold && nextGCThreshold) {
        if (images.getUsedMemory() > nextGCThreshold) {
            images.gc();
            nextGCThreshold = images.getUsedMemory() + gcThreshold;
        }
    }
    this._handle = new _Image(width, height);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.images.copyFromImage"></a>[function <span class="apidocSignatureSpan">images.</span>copyFromImage (src, x, y, width, height)](#apidoc.element.images.copyFromImage)
- description and source-code
```javascript
copyFromImage = function (src, x, y, width, height) {
    return WrappedImage().copyFromImage(src, x, y, width, height);
}
```
- example usage
```shell
...
loadFromBuffer: function(buffer, start, end) {
    this._handle.loadFromBuffer(buffer, start, end);
},
copyFromImage: function(img, x, y, width, height) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.copyFromImage(img, x, y, width, height);
},
fill: function(red, green, blue, alpha) {
    this._handle.fillColor(red, green, blue, alpha);
},
draw: function(img, x, y) {
    if (img instanceof WrappedImage) {
        img = img._handle;
...
```

#### <a name="apidoc.element.images.createImage"></a>[function <span class="apidocSignatureSpan">images.</span>createImage (width, height)](#apidoc.element.images.createImage)
- description and source-code
```javascript
createImage = function (width, height) {
    return WrappedImage(width, height);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.images.gc"></a>[function <span class="apidocSignatureSpan">images.</span>gc ()](#apidoc.element.images.gc)
- description and source-code
```javascript
gc = function () {
    return _images.gc();
}
```
- example usage
```shell
...
Set the garbage collection threshold
设置图像处理库自动gc的阈值(当*新增*内存使用超过该阈值时，执行垃圾回收)

### images.getUsedMemory()
Get used memory (in bytes)
得到图像处理库占用的内存大小(单位为字节)

### images.gc()
Forced call garbage collection
强制调用V8的垃圾回收机制
...
```

#### <a name="apidoc.element.images.getUsedMemory"></a>[function <span class="apidocSignatureSpan">images.</span>getUsedMemory ()](#apidoc.element.images.getUsedMemory)
- description and source-code
```javascript
getUsedMemory = function () {
    return _images.usedMemory;
}
```
- example usage
```shell
...
Set the limit size of each image
设置库处理图片的大小限制,设置后对所有新的操作生效(如果超限则抛出异常)

### images.setGCThreshold(value)
Set the garbage collection threshold
设置图像处理库自动gc的阈值(当*新增*内存使用超过该阈值时，执行垃圾回收)

### images.getUsedMemory()
Get used memory (in bytes)
得到图像处理库占用的内存大小(单位为字节)

### images.gc()
Forced call garbage collection
强制调用V8的垃圾回收机制
...
```

#### <a name="apidoc.element.images.loadFromBuffer"></a>[function <span class="apidocSignatureSpan">images.</span>loadFromBuffer (buffer, start, end)](#apidoc.element.images.loadFromBuffer)
- description and source-code
```javascript
loadFromBuffer = function (buffer, start, end) {
    return WrappedImage().loadFromBuffer(buffer, start, end);
}
```
- example usage
```shell
...
    }
}
this._handle = new _Image(width, height);
}

prototype = {
loadFromBuffer: function(buffer, start, end) {
    this._handle.loadFromBuffer(buffer, start, end);
},
copyFromImage: function(img, x, y, width, height) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.copyFromImage(img, x, y, width, height);
},
...
```

#### <a name="apidoc.element.images.loadFromFile"></a>[function <span class="apidocSignatureSpan">images.</span>loadFromFile (file)](#apidoc.element.images.loadFromFile)
- description and source-code
```javascript
loadFromFile = function (file) {
    return images.loadFromBuffer(fs.readFileSync(file));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.images.setGCThreshold"></a>[function <span class="apidocSignatureSpan">images.</span>setGCThreshold (value)](#apidoc.element.images.setGCThreshold)
- description and source-code
```javascript
setGCThreshold = function (value) {
    gcThreshold = value;
    nextGCThreshold = value;
}
```
- example usage
```shell
...
Get height for the image or set height of the image
获取或设置图像高度

### images.setLimit(width, height)
Set the limit size of each image
设置库处理图片的大小限制,设置后对所有新的操作生效(如果超限则抛出异常)

### images.setGCThreshold(value)
Set the garbage collection threshold
设置图像处理库自动gc的阈值(当*新增*内存使用超过该阈值时，执行垃圾回收)

### images.getUsedMemory()
Get used memory (in bytes)
得到图像处理库占用的内存大小(单位为字节)
...
```

#### <a name="apidoc.element.images.setLimit"></a>[function <span class="apidocSignatureSpan">images.</span>setLimit (maxWidth, maxHeight)](#apidoc.element.images.setLimit)
- description and source-code
```javascript
setLimit = function (maxWidth, maxHeight) {
    _images.maxHeight = maxHeight;
    _images.maxWidth = maxWidth;
    return images;
}
```
- example usage
```shell
...
Get width for the image or set width of the image
获取或设置图像宽度

### .height([height])
Get height for the image or set height of the image
获取或设置图像高度

### images.setLimit(width, height)
Set the limit size of each image
设置库处理图片的大小限制,设置后对所有新的操作生效(如果超限则抛出异常)

### images.setGCThreshold(value)
Set the garbage collection threshold
设置图像处理库自动gc的阈值(当*新增*内存使用超过该阈值时，执行垃圾回收)
...
```



# <a name="apidoc.module.images.Image"></a>[module images.Image](#apidoc.module.images.Image)

#### <a name="apidoc.element.images.Image.Image"></a>[function <span class="apidocSignatureSpan">images.</span>Image (width, height)](#apidoc.element.images.Image.Image)
- description and source-code
```javascript
function WrappedImage(width, height) {
    if (!(this instanceof WrappedImage)) return new WrappedImage(width, height);
    if (gcThreshold && nextGCThreshold) {
        if (images.getUsedMemory() > nextGCThreshold) {
            images.gc();
            nextGCThreshold = images.getUsedMemory() + gcThreshold;
        }
    }
    this._handle = new _Image(width, height);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.images.Image.prototype"></a>[module images.Image.prototype](#apidoc.module.images.Image.prototype)

#### <a name="apidoc.element.images.Image.prototype.copyFromImage"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>copyFromImage ()](#apidoc.element.images.Image.prototype.copyFromImage)
- description and source-code
```javascript
copyFromImage = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
loadFromBuffer: function(buffer, start, end) {
    this._handle.loadFromBuffer(buffer, start, end);
},
copyFromImage: function(img, x, y, width, height) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.copyFromImage(img, x, y, width, height);
},
fill: function(red, green, blue, alpha) {
    this._handle.fillColor(red, green, blue, alpha);
},
draw: function(img, x, y) {
    if (img instanceof WrappedImage) {
        img = img._handle;
...
```

#### <a name="apidoc.element.images.Image.prototype.draw"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>draw ()](#apidoc.element.images.Image.prototype.draw)
- description and source-code
```javascript
draw = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
''' javascript
var images = require("images");

images("input.jpg")                     //Load image from file
                                        //加载图像文件
    .size(400)                          //Geometric scaling the image to 400 pixels width
                                        //等比缩放图像到400像素宽
    .draw(images("logo.png"), 10, 10)   //Drawn logo at coordinates (10,10)
                                        //在(10,10)处绘制Logo
    .save("output.jpg", {               //Save the image to a file,whih quality 50
        quality : 50                    //保存图片到文件,图片质量为50
	});
'''
## Features 功能特性
...
```

#### <a name="apidoc.element.images.Image.prototype.drawImage"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>drawImage ()](#apidoc.element.images.Image.prototype.drawImage)
- description and source-code
```javascript
drawImage = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
fill: function(red, green, blue, alpha) {
    this._handle.fillColor(red, green, blue, alpha);
},
draw: function(img, x, y) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.drawImage(img, x, y);
},
encode: function(type, config) {
    var configurator;
    if (typeof(type) != "number") {
        type = String(type).toLowerCase();
        type = (FILE_TYPE_MAP["." + type] || FILE_TYPE_MAP[type]);
    }
...
```

#### <a name="apidoc.element.images.Image.prototype.encode"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>encode ()](#apidoc.element.images.Image.prototype.encode)
- description and source-code
```javascript
encode = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
Fill image with color
以指定颜色填充图像

### .draw(image, x, y)
Draw *image* on the current image position( *x* , *y* )
在当前图像( *x* , *y* )上绘制 *image* 图像

### .encode(type[, config])
eg:'images("input.png").encode("jpg", {operation:50})'
Encode image to buffer, *config* is image setting.
以指定格式编码当前图像到Buffer，config为图片设置，目前支持设置JPG图像质量
Return buffer
返回填充好的Buffer
**Note:The operation will cut off the chain**
**注意:该操作将会切断调用链**
...
```

#### <a name="apidoc.element.images.Image.prototype.fill"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>fill ()](#apidoc.element.images.Image.prototype.fill)
- description and source-code
```javascript
fill = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
Load and decode image from a buffer
从Buffer数据中解码图像

### images(image[, x, y, width, height])
Copy from another image
从另一个图像中复制区域来创建图像

### .fill(red, green, blue[, alpha])
eg:'images(200, 100).fill(0xff, 0x00, 0x00, 0.5)'
Fill image with color
以指定颜色填充图像

### .draw(image, x, y)
Draw *image* on the current image position( *x* , *y* )
在当前图像( *x* , *y* )上绘制 *image* 图像
...
```

#### <a name="apidoc.element.images.Image.prototype.fillColor"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>fillColor ()](#apidoc.element.images.Image.prototype.fillColor)
- description and source-code
```javascript
fillColor = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
copyFromImage: function(img, x, y, width, height) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.copyFromImage(img, x, y, width, height);
},
fill: function(red, green, blue, alpha) {
    this._handle.fillColor(red, green, blue, alpha);
},
draw: function(img, x, y) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.drawImage(img, x, y);
},
...
```

#### <a name="apidoc.element.images.Image.prototype.height"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>height ()](#apidoc.element.images.Image.prototype.height)
- description and source-code
```javascript
height = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
Set the size of the image,if the height is not specified, then scaling based on the current width and height
设置图像宽高，如果height未指定，则根据当前宽高等比缩放, 默认采用 bicubic 算法。

### .width([width])
Get width for the image or set width of the image
获取或设置图像宽度

### .height([height])
Get height for the image or set height of the image
获取或设置图像高度

### images.setLimit(width, height)
Set the limit size of each image
设置库处理图片的大小限制,设置后对所有新的操作生效(如果超限则抛出异常)
...
```

#### <a name="apidoc.element.images.Image.prototype.loadFromBuffer"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>loadFromBuffer ()](#apidoc.element.images.Image.prototype.loadFromBuffer)
- description and source-code
```javascript
loadFromBuffer = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
    }
}
this._handle = new _Image(width, height);
}

prototype = {
loadFromBuffer: function(buffer, start, end) {
    this._handle.loadFromBuffer(buffer, start, end);
},
copyFromImage: function(img, x, y, width, height) {
    if (img instanceof WrappedImage) {
        img = img._handle;
    }
    this._handle.copyFromImage(img, x, y, width, height);
},
...
```

#### <a name="apidoc.element.images.Image.prototype.resize"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>resize ()](#apidoc.element.images.Image.prototype.resize)
- description and source-code
```javascript
resize = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
Encoding and save the current image to a *file*, if the *type* is not specified, *type* well be automatically determined according
 to the *file*, *config* is image setting. eg: '{ operation:50 }'
编码并保存当前图像到 *file* ,如果type未指定,则根据 *file* 自动判断文件类型，config为图片设置，目前支持设置JPG图像质量

### .size([width[, height]])
Get size of the image or set the size of the image,if the height is not specified, then scaling based on the current width and height
获取或者设置图像宽高，如果height未指定，则根据当前宽高等比缩放

### .resize(width[, height])
Set the size of the image,if the height is not specified, then scaling based on the current width and height
设置图像宽高，如果height未指定，则根据当前宽高等比缩放, 默认采用 bicubic 算法。

### .width([width])
Get width for the image or set width of the image
获取或设置图像宽度
...
```

#### <a name="apidoc.element.images.Image.prototype.save"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>save ()](#apidoc.element.images.Image.prototype.save)
- description and source-code
```javascript
save = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...

images("input.jpg")                     //Load image from file
                                        //加载图像文件
    .size(400)                          //Geometric scaling the image to 400 pixels width
                                        //等比缩放图像到400像素宽
    .draw(images("logo.png"), 10, 10)   //Drawn logo at coordinates (10,10)
                                        //在(10,10)处绘制Logo
    .save("output.jpg", {               //Save the image to a file,whih quality 50
        quality : 50                    //保存图片到文件,图片质量为50
	});
'''
## Features 功能特性

* Lightweight:no need to install any image processing library.
* 轻量级：无需安装任何图像处理库。
...
```

#### <a name="apidoc.element.images.Image.prototype.saveAsync"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>saveAsync ()](#apidoc.element.images.Image.prototype.saveAsync)
- description and source-code
```javascript
saveAsync = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.images.Image.prototype.size"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>size ()](#apidoc.element.images.Image.prototype.size)
- description and source-code
```javascript
size = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
Node.js轻量级跨平台图像编解码库

''' javascript
var images = require("images");

images("input.jpg")                     //Load image from file
                                        //加载图像文件
    .size(400)                          //Geometric scaling the image to 400 pixels width
                                        //等比缩放图像到400像素宽
    .draw(images("logo.png"), 10, 10)   //Drawn logo at coordinates (10,10)
                                        //在(10,10)处绘制Logo
    .save("output.jpg", {               //Save the image to a file,whih quality 50
        quality : 50                    //保存图片到文件,图片质量为50
	});
'''
...
```

#### <a name="apidoc.element.images.Image.prototype.toBuffer"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>toBuffer ()](#apidoc.element.images.Image.prototype.toBuffer)
- description and source-code
```javascript
toBuffer = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
        type = String(type).toLowerCase();
        type = (FILE_TYPE_MAP["." + type] || FILE_TYPE_MAP[type]);
    }
    if (config != undefined) {
        configurator = CONFIG_GENERATOR[type];
        config = configurator && configurator(config);
    }
    return this._handle.toBuffer(type, config);
},
save: function(file, type, config) {
    if (type && typeof(type) == "object") {
        config = type;
        type = undefined;
    }
    fs.writeFileSync(file, this.encode(type || path.extname(file), config));
...
```

#### <a name="apidoc.element.images.Image.prototype.width"></a>[function <span class="apidocSignatureSpan">images.Image.prototype.</span>width ()](#apidoc.element.images.Image.prototype.width)
- description and source-code
```javascript
width = function () {
    var ret = fn.apply(this, slice.call(arguments, 0));
    return ret === undefined ? this : ret;
}
```
- example usage
```shell
...
Get size of the image or set the size of the image,if the height is not specified, then scaling based on the current width and height
获取或者设置图像宽高，如果height未指定，则根据当前宽高等比缩放

### .resize(width[, height])
Set the size of the image,if the height is not specified, then scaling based on the current width and height
设置图像宽高，如果height未指定，则根据当前宽高等比缩放, 默认采用 bicubic 算法。

### .width([width])
Get width for the image or set width of the image
获取或设置图像宽度

### .height([height])
Get height for the image or set height of the image
获取或设置图像高度
...
```



# <a name="apidoc.module.images.binding"></a>[module images.binding](#apidoc.module.images.binding)

#### <a name="apidoc.element.images.binding.Image"></a>[function <span class="apidocSignatureSpan">images.binding.</span>Image ()](#apidoc.element.images.binding.Image)
- description and source-code
```javascript
function Image() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.images.binding.gc"></a>[function <span class="apidocSignatureSpan">images.binding.</span>gc ()](#apidoc.element.images.binding.gc)
- description and source-code
```javascript
function gc() { [native code] }
```
- example usage
```shell
...
Set the garbage collection threshold
设置图像处理库自动gc的阈值(当*新增*内存使用超过该阈值时，执行垃圾回收)

### images.getUsedMemory()
Get used memory (in bytes)
得到图像处理库占用的内存大小(单位为字节)

### images.gc()
Forced call garbage collection
强制调用V8的垃圾回收机制
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
