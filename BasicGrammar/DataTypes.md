# 数据类型

```
	var PI0 float32 = 3.14
	fmt.Println(PI0)
    <!-- 变量的数据类型 -->
	fmt.Printf("%T \n", PI0)
    <!-- 变量的数据字节数 -->
	fmt.Println(unsafe.Sizeof(PI0), "byte")
```

## 1. 布尔型

`var b bool = true`

## 2. 数值类型

整型 int 和浮点型 float32、float64（支持复数，其中位的运算采用补码）

```
uint: uint8、uint16、uint32、uint64

int: int8、int16、int32、int64

byte：类似 uint8

rune：类似 int32

int/uint：32 或 64 位

uintpt：无符号整型，用于存放一个指针

float32：32位浮点型数

float64：64位浮点型数

complex64：32 位实数和虚数

complex128：64 位实数和虚数
```

## 3. 字符串类型

`var name string`

## 4. 派生类型

### (a) 指针类型（Pointer）

### (b) 数组类型

### (c) 结构化类型(struct)

### (d) Channel 类型

### (e) 函数类型

### (f) 切片类型

### (g) 接口类型（interface）

### (h) Map 类型

# 变量 var

变量声明并赋值：`var age2 int = 3`

## 1. 变量声明

### (1) 指定变量类型

`如果没有初始化，则变量默认为零值`

```
var age int
age = 20
```

### (2) 根据值自行判定变量类型

```
var name ="zhangsan"
```

### (3) 省略 var，使用 `:=` 声明变量

```
intVal := 100
```

## 2.多变量声明

```
// 先声明再赋值
var n1, n2, n3 int
n1, n2, n3 = 1, 2, 3

// 自行判定变量类型
var v1, v2, v3 = 10, true, "zhan"

// :=
m1, m2, m3 := 10, 15.4, false
```

## 3.全局变量的声明

var (
name = "A"
age = 18
)

```
package main

import "fmt"

// 全局变量
var (
	name = "A"
	age  = 18
)

func main() {

	fmt.Println(name, age)

}
```

# 常量 const

```
const b string = "abc"

or

const b = "abc"
```
