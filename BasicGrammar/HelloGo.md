```go
package main

import "fmt"

func init() {
	fmt.Println("First")
}
func main() {
	fmt.Println("Hello Go!")
}
```

1. `必须`在源文件中第一行`指明`这个文件`属于哪个包`

2. `import "fmt"` 告诉 Go 编译器这个程序需要使用 fmt 包

3. `main 函数`是每一个可执行程序所`必须包含`的，一般来说都是在启动后第一个执行的函数（如果有 init() 函数则会先执行该函数）

4. `fmt.Println(...)` 可以将字符串输出到控制台，并在最后自动增加换行字符 \n
