```js
class Point3 extends Point2 {
  constructor(x, y, z) { super(x, y); this.z = z }
  foobar() { return this.x }
  callSuper() { return super.hello() }
}

class Point2 {
  constructor(x, y) { this.x = x; this.y = y }
  hello() { return "hello" }
}

var p = new Point3(1, 2, 3)
p.x //: number
p.hello() //: string
p.callSuper() //: string
p.foobar() //: number

var pro = {x: 10}

var obj = {
  __proto__: pro,
  x: "string",
  getSuperX() { return super.x }
}

obj.x //: string
obj.getSuperX() //: number
```
```json
[
  {
    "id": "24496120-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "Point3",
    "addr": "/Point3/",
    "kind": "f",
    "type": "void function(number, number, number)",
    "lineno": 1,
    "origin": {
      "!span": "6[0:6]-12[0:12]",
      "!type": "fn(x: number, y: number, z: number)",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "2449d650-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "prototype",
    "addr": "/class Point3 extends Point2 \{/",
    "kind": "v",
    "lineno": 1,
    "namespace": "Point3",
    "parent": "24496120-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "0[0:0]-150[4:1]",
      "!data": {
        "isConstructor": false,
        "type": "Point2.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "2449fd62-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "z",
    "addr": "/z/",
    "kind": "v",
    "type": "number",
    "lineno": 2,
    "namespace": "Point3",
    "parent": "24496120-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "73[1:43]-74[1:44]",
      "!type": "number",
      "!data": {
        "isConstructor": false,
        "type": "Number.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "2449fd60-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "foobar",
    "addr": "/foobar/",
    "kind": "f",
    "type": "!this.x function()",
    "lineno": 3,
    "namespace": "Point3.prototype",
    "parent": "2449d650-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "83[2:2]-89[2:8]",
      "!type": "fn() -> !this.x",
      "!data": {
        "isConstructor": false,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "2449fd61-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "callSuper",
    "addr": "/callSuper/",
    "kind": "f",
    "type": "string function()",
    "lineno": 4,
    "namespace": "Point3.prototype",
    "parent": "2449d650-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "112[3:2]-121[3:11]",
      "!type": "fn() -> string",
      "!data": {
        "isConstructor": false,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2472-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "prototype",
    "addr": "/class Point2 \{/",
    "kind": "v",
    "lineno": 7,
    "namespace": "Point2",
    "parent": "244a2471-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "152[6:0]-244[9:1]",
      "!data": {
        "isConstructor": false,
        "type": "Object.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2471-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "Point2",
    "addr": "/Point2/",
    "kind": "f",
    "type": "void function(number, number)",
    "lineno": 7,
    "origin": {
      "!span": "158[6:6]-164[6:12]",
      "!type": "fn(x: number, y: number)",
      "!data": {
        "isConstructor": true,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2470-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "y",
    "addr": "/y/",
    "kind": "v",
    "type": "number",
    "lineno": 8,
    "namespace": "Point3",
    "parent": "24496120-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "206[7:39]-207[7:40]",
      "!type": "number",
      "!data": {
        "isConstructor": false,
        "type": "Number.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "2449fd63-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "x",
    "addr": "/x/",
    "kind": "v",
    "type": "number",
    "lineno": 8,
    "namespace": "Point3",
    "parent": "24496120-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "194[7:27]-195[7:28]",
      "!type": "number",
      "!data": {
        "isConstructor": false,
        "type": "Number.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2473-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "hello",
    "addr": "/hello/",
    "kind": "f",
    "type": "string function()",
    "lineno": 9,
    "namespace": "Point2.prototype",
    "parent": "244a2472-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "216[8:2]-221[8:7]",
      "!type": "fn() -> string",
      "!data": {
        "isConstructor": false,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2474-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "p",
    "addr": "/p/",
    "kind": "v",
    "type": "Point3",
    "lineno": 12,
    "origin": {
      "!span": "250[11:4]-251[11:5]",
      "!type": "+Point3",
      "!data": {
        "isConstructor": false,
        "type": "Point3.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2475-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "pro",
    "addr": "/pro/",
    "kind": "v",
    "lineno": 18,
    "origin": {
      "!span": "362[17:4]-365[17:7]",
      "!data": {
        "isConstructor": false,
        "type": "Object.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2476-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "x",
    "addr": "/x/",
    "kind": "v",
    "type": "number",
    "lineno": 18,
    "namespace": "pro",
    "parent": "244a2475-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "369[17:11]-370[17:12]",
      "!type": "number",
      "!data": {
        "isConstructor": false,
        "type": "Number.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2477-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "obj",
    "addr": "/obj/",
    "kind": "v",
    "lineno": 20,
    "origin": {
      "!span": "381[19:4]-384[19:7]",
      "!data": {
        "isConstructor": false,
        "type": "pro"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2478-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "x",
    "addr": "/x/",
    "kind": "v",
    "type": "string",
    "lineno": 22,
    "namespace": "obj",
    "parent": "244a2477-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "409[21:2]-410[21:3]",
      "!type": "string",
      "!data": {
        "isConstructor": false,
        "type": "String.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  },
  {
    "id": "244a2479-7aef-11e6-89a5-adcd23ba8aaf",
    "name": "getSuperX",
    "addr": "/getSuperX/",
    "kind": "f",
    "type": "number function()",
    "lineno": 23,
    "namespace": "obj",
    "parent": "244a2477-7aef-11e6-89a5-adcd23ba8aaf",
    "origin": {
      "!span": "424[22:2]-433[22:11]",
      "!type": "fn() -> number",
      "!data": {
        "isConstructor": false,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/super.js"
  }
]
```
```ctags
Point3	__DIR__/super.js	/Point3/;"	f	lineno:1	type:void function(number, number, number)
prototype	__DIR__/super.js	/class Point3 extends Point2 \{/;"	v	lineno:1	namespace:Point3
z	__DIR__/super.js	/z/;"	v	lineno:2	namespace:Point3	type:number
foobar	__DIR__/super.js	/foobar/;"	f	lineno:3	namespace:Point3.prototype	type:!this.x function()
callSuper	__DIR__/super.js	/callSuper/;"	f	lineno:4	namespace:Point3.prototype	type:string function()
prototype	__DIR__/super.js	/class Point2 \{/;"	v	lineno:7	namespace:Point2
Point2	__DIR__/super.js	/Point2/;"	f	lineno:7	type:void function(number, number)
y	__DIR__/super.js	/y/;"	v	lineno:8	namespace:Point3	type:number
x	__DIR__/super.js	/x/;"	v	lineno:8	namespace:Point3	type:number
hello	__DIR__/super.js	/hello/;"	f	lineno:9	namespace:Point2.prototype	type:string function()
p	__DIR__/super.js	/p/;"	v	lineno:12	type:Point3
pro	__DIR__/super.js	/pro/;"	v	lineno:18
x	__DIR__/super.js	/x/;"	v	lineno:18	namespace:pro	type:number
obj	__DIR__/super.js	/obj/;"	v	lineno:20
x	__DIR__/super.js	/x/;"	v	lineno:22	namespace:obj	type:string
getSuperX	__DIR__/super.js	/getSuperX/;"	f	lineno:23	namespace:obj	type:number function()
```
