# acolor

```
;(function(root){
let em='black,blue,red,purple,green,skyblue,yellow,white'.split(',')
let ary=[
 ['#fff','#ddd','#bbb','#999','#777','#555','#333','#000']
,['#001','#003','#005','#007','#009','#00b','#00d','#00f']
,['#100','#300','#500','#700','#900','#b00','#d00','#f00']
,['#101','#303','#505','#707','#909','#b0b','#d0d','#f0f']
,['#010','#030','#050','#070','#090','#0b0','#0d0','#0f0']
,['#011','#033','#055','#077','#099','#0bb','#0dd','#0ff']
,['#110','#330','#550','#770','#990','#bb0','#dd0','#ff0']
,['#111','#333','#555','#777','#999','#bbb','#ddd','#fff']
];

em.map((d,i)=>{
 root[d]=function(v){return ary[i][Math.min(v,7)]}
})
let usage=`
black(0) black(7)
blue
red
purple
green
skyblue
yellow
white
`
console.log('usage',usage)
})(this); 
```
